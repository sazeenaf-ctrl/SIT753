// Updated to test auto-trigger
pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Stage 1: Build'
                echo 'Tool: Maven'
                echo 'Task: Compiling and packaging the application using Maven build automation tool.'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Tool: JUnit (unit tests), Selenium (integration tests)'
                echo 'Task: Running unit tests to verify individual components and integration tests to ensure modules work together.'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Tool: SonarQube'
                echo 'Task: Analysing source code for bugs, code smells, and ensuring it meets industry coding standards.'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Tool: OWASP Dependency Check'
                echo 'Task: Scanning code and dependencies for known security vulnerabilities and CVEs.'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Tool: AWS CLI / Ansible'
                echo 'Task: Deploying the packaged application to an AWS EC2 staging instance for pre-production testing.'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Tool: Selenium / Postman'
                echo 'Task: Running integration tests on the staging environment to verify the application works in a production-like setup.'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Tool: AWS CLI / Ansible'
                echo 'Task: Deploying the verified application to the live AWS EC2 production server.'
            }
        }
    }
}
