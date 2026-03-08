# Getting Started
To build and run this project you will require the following:
* Java 18 (or higher)
* Maven 3.6.3 (or higher)

## Running automated checks for the project
The project contains Unit, API and E2E  checks.
The automated checks in this project can be run in two ways.

## Running Unit and API checks
To run these checks, run the following command in the root of the project:

`mvn clean verify`

## Running E2E checks
E2E checks are run after the application is built. To run these checks, run the following command in the root of the project:

`mvn test -Dtest=LoginTest`

## CI/CD Integration
This project is integrated with GitHub Actions. The build and test process is triggered everytime a change is pushed to the main branch.

The config file for Actions can be found in the following location:

`github/workflows/build_test_maven.yml`

Workflow outputs can be found in the Actions section of the GitHub repository.

## Building the project
To build the project simply run `mvn clean install` to create a jar file in the target directory.

## Running the project
To run the project simply run `java -jar target/mot-cert-support-app-java-*-exec.jar` to run the jar file. 

