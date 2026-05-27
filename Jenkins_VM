pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                url: 'https://github.com/Suvetha-E/sample-java-app.git'
            }
        }
        stage('Build') {
            steps {
                bat 'echo Building Application'
            }
        }
        stage('Test') {
            steps {
                bat 'echo Running Tests'
            }
        }
    }
    post {
        success {
            echo 'Pipeline Executed Successfully'
        }
        failure {
            echo 'Pipeline Failed'
        }
    }
}
