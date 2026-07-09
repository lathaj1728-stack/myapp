pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'python3 --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'python3 -m pip install --break-system-packages pytest'
            }
        }

        stage('Test') {
            steps {
                sh 'python3 -m pytest'
            }
        }
    }
}