pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                bat '"C:\\Users\\Bhargavi\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" -m pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                bat '"C:\\Users\\Bhargavi\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" -m pytest'
            }
        }

        stage('Build Success') {
            steps {
                echo 'Build completed successfully!'
            }
        }
    }
}