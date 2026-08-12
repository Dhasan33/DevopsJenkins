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
                sh 'echo "BUILD SUCCESSFUL"'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo "ALL TESTS PASSED"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying demo application...'
                sh 'echo "DEPLOYMENT SUCCESSFUL"'
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
