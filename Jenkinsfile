pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out source code...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage executed'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                echo 'All tests passed'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment stage executed'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
