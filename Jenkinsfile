pipeline {
    agent any

    tools {
        maven "M2"
        jdk "JAVA_HOME"
    }

    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/sushant960kr/DevOpsClassCodes.git'

                // Use Maven build command for Windows
                bat 'mvn -Dmaven.test.failure.ignore=true clean package'
            }
        }

        stage('Compile') {
            steps {
                bat 'mvn compile'
            }   
        }

        stage('Code Review') {
            steps {
                bat 'mvn pmd:pmd'
            }
            post {
                success {
                    recordIssues sourceCodeRetention: 'LAST_BUILD', tools: [pmdParser(pattern: '**/pmd.xml')]
                }
            }
            
        }

        

        stage('Code Package') {
            steps {
                bat 'mvn package'
            }
        }
    }
}
