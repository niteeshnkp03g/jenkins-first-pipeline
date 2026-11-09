pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Starting Jenkins Pipeline'
                echo 'Checking out GitHub repository'
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage executed successfully'
            }
        }

        stage('Test') {
            steps {
                echo 'Test stage executed successfully'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy stage executed successfully'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }

        failure {
            echo 'Pipeline failed!'
        }
    }
}