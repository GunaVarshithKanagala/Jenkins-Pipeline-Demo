pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building code with Maven...'
                sh 'echo "Maven: mvn clean package"'
            }
        }
        
        stage('Unit and Integration Tests') {
            steps {
                echo 'Running unit and integration tests...'
                sh 'echo "JUnit: Running tests"'
            }
        }
        
        stage('Code Analysis') {
            steps {
                echo 'Analyzing code...'
                sh 'echo "SonarQube: Code analysis"'
            }
        }
        
        stage('Security Scan') {
            steps {
                echo 'Performing security scan...'
                sh 'echo "OWASP ZAP: Security scan"'
            }
        }
        
        stage('Deploy to Staging') {
            steps {
                echo 'Deploying to staging server...'
                sh 'echo "AWS EC2: Deploy to staging"'
            }
        }
        
        stage('Integration Tests on Staging') {
            steps {
                echo 'Running integration tests on staging...'
                sh 'echo "Postman: Integration tests"'
            }
        }
        
        stage('Deploy to Production') {
            steps {
                echo 'Deploying to production...'
                sh 'echo "AWS EC2: Deploy to production"'
            }
        }
    }
}
