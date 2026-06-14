pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                echo 'Code pulled from GitHub'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'pytest'
            }
        }

        stage('Build Success') {
            steps {
                echo 'Python Flask app tested successfully!'
            }
        }
    }
}