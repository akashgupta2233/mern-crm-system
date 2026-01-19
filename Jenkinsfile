pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/hemantsinghdev/crm-system.git'
            }
        }

        stage('Install Backend Dependencies') {
            steps {
                dir('client-api') {
                    sh 'npm install'
                }
            }
        }

        stage('Install Frontend Dependencies') {
            steps {
                dir('frontend') {
                    sh 'npm install'
                }
            }
        }

        stage('Build Docker Images') {
            steps {
                sh 'docker build -t crm-backend ./client-api'
                sh 'docker build -t crm-frontend ./frontend'
            }
        }
    }
}
