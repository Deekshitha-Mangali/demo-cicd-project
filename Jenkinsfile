pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building the application...'
                bat 'python --version'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the application...'
                bat 'python app.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Application deployment completed!'
            }
        }
    }

    post {
        success {
            echo 'CI/CD Pipeline completed successfully!'
        }

        failure {
            echo 'CI/CD Pipeline failed.'
        }
    }
}
