pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Downloading source code from GitHub'
            }
        }

        stage('Build') {
            steps {
                echo 'Checking Linux environment'
                sh 'whoami'
                sh 'pwd'
                sh 'git --version'
            }
        }

        stage('Test') {
            steps {
                echo 'Checking project files'
                sh 'ls -la'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment preparation completed'
            }
        }
    }

    post {
        success {
            echo 'CI/CD Pipeline completed successfully!'
        }

        failure {
            echo 'Pipeline execution failed!'
        }
    }
}