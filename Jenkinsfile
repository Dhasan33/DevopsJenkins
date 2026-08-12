pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Source code checked out from GitHub'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                bat 'echo BUILD SUCCESSFUL'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'echo ALL TESTS PASSED'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying demo application...'
                bat 'echo DEPLOYMENT SUCCESSFUL'
            }
        }
    }

    post {
        success {
            echo 'Jenkins pipeline completed successfully!'
        }

        failure {
            echo 'Jenkins pipeline failed!'
        }
    }
}
