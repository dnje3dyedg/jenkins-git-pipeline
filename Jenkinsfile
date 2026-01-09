pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Code cloned from GitHub'
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage running'
            }
        }

        stage('Run') {
            steps {
                sh 'bash app.sh'
            }
        }
    }
}
