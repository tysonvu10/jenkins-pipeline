pipeline {
    agent any

    triggers {
        pollSCM('H/5 * * * *')
    }

    stages {
        stage('Build') {
            steps {
                echo "Stage 1: Build"
                echo "Task: Build the code using Maven to compile and package the application."
                echo "Tool: Maven"
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo "Stage 2: Unit and Integration Tests"
                echo "Task: Run unit tests using JUnit to ensure the code functions as expected."
                echo "Task: Run integration tests using Selenium to ensure components work together."
                echo "Tool: JUnit (unit tests), Selenium (integration tests)"
            }
        }
        stage('Code Analysis') {
            steps {
                echo "Stage 3: Code Analysis"
                echo "Task: Analyse the code using SonarQube to ensure it meets industry standards."
                echo "Tool: SonarQube"
            }
        }
        stage('Security Scan') {
            steps {
                echo "Stage 4: Security Scan"
                echo "Task: Perform a security scan using OWASP Dependency-Check to identify vulnerabilities."
                echo "Tool: OWASP Dependency-Check"
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo "Stage 5: Deploy to Staging"
                echo "Task: Deploy the application to a staging server (AWS EC2 instance)."
                echo "Tool: AWS CLI"
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo "Stage 6: Integration Tests on Staging"
                echo "Task: Run integration tests on the staging environment using Selenium."
                echo "Tool: Selenium"
            }
        }
        stage('Deploy to Production') {
            steps {
                echo "Stage 7: Deploy to Production"
                echo "Task: Deploy the application to a production server (AWS EC2 instance)."
                echo "Tool: AWS CLI"
            }
        }
    }
}
//updated
