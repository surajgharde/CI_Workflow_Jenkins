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
                echo 'Installing dependencies...'
                sh 'pip3 install -r requirements.txt'
            }
        }

        stage('Test') {
            steps {
                sh 'python3 -m unittest test_app.py'
            }
        }
    }
}