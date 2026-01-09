pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Cloning repository from GitHub'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage running'
            }
        }

        stage('Run') {
            steps {
                echo 'Executing application'
                bat 'app.bat'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}

