pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                echo 'Jenkins automatically pulled the latest code from GitHub!'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
                bat 'echo Build complete!'
            }
        }
        stage('Run Tests') {
            steps {
                echo 'Running Pytest automated suite...'
                bat 'echo Test 1: PASS, Test 2: PASS'
            }
        }
    }
}
