pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                echo 'Code already checked out by Jenkins'
            }
        }

        stage('Build') {
            steps {
                echo 'Building application...'
            }
        }

        stage('Test') {
            steps {
                sh 'python -m unittest test_app.py'
            }
        }
    }
}