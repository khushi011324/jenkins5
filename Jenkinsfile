pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code from the repository'
                script {
                    // Checkout code from Git repository
                    git branch: 'main', url: 'https://github.com/khushi011324/jenkins5.git'
                }
            }
        }
        
        stage('Build') {
            steps {
                echo 'Starting Build stage using Maven'
               
            }
        }
        
        stage('Unit and Integration Tests') {
            steps {
                echo 'Starting Unit and Integration Tests stage using TestNG'
                emailext attachLog: true, body: 'uyhgtfr', subject: 'hu', to: 'khushi131721@gmail.com'
                
            }
        }
        
        stage('Code Analysis') {
            steps {
                echo 'Starting Code Analysis stage using SonarQube'
            }
        }
        
        stage('Security Scan') {
            steps {
                echo 'Starting Security Scan stage using SonarQube'
                 emailext attachLog: true, body: 'uyhgtfr', subject: 'hu', to: 'khushi131721@gmail.com'
            }
        }
        
        stage('Deploy to Staging') {
            steps {
                echo 'Starting Deploy to Staging stage using Docker'
            }
        }
        
        stage('Integration Tests on Staging') {
            steps {
                echo 'Starting Integration Tests on Staging stage using Selenium'
            }
        }
        
        stage('Deploy to Production') {
            steps {
                echo 'Starting Deploy to Production stage using Docker'
            }
        }
    }
}
