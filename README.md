# Jenkins Pipeline for DevOps Class Codes

This repository contains a Jenkins pipeline configuration for building, testing, and packaging Java applications using Maven.

## Table of Contents
- [Overview](#overview)
- [Pipeline Stages](#pipeline-stages)
- [Prerequisites](#prerequisites)
- [How to Use](#how-to-use)
- [Contributing](#contributing)

## Overview
This Jenkins pipeline automates the process of building, testing, and packaging a Java application. It includes code review using PMD and generates test reports.

## Pipeline Stages
1. **Build**: Clones the repository and builds the project using Maven.
2. **Compile**: Compiles the Java source code.
3. **Code Review**: Runs PMD for static code analysis.
4. **Code Test**: Executes unit tests and generates test reports.
5. **Code Package**: Packages the application into a deployable format.

## Prerequisites
- Jenkins server with the following tools installed:
  - Maven (configured as "M2")
  - JDK (configured as "JAVA_HOME")

## How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/sushant960kr/DevOpsClassCodes.git

![Screenshot 2024-09-22 093005](https://github.com/user-attachments/assets/a4d8605c-210d-4577-bad0-4c3c5db312eb)
![Screenshot 2024-09-22 093045](https://github.com/user-attachments/assets/afb01e12-5b58-4f09-ab75-2f99149bc064)
![Screenshot 2024-09-22 092841](https://github.com/user-attachments/assets/90afc3ad-fbdb-4bd4-ad1d-b70b229c11a9)
