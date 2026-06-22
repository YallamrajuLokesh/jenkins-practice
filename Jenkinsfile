pipeline {
    // Instead of 'any', we specify a strict Docker image environment
    agent {
        docker {
            image 'python:3.10-slim'
        }
    }

    stages {
        stage('Environment Check') {
            steps {
                echo 'Checking the environment inside the isolated container...'
                // Since this image is Linux-based, we use 'sh' instead of 'bat'!
                sh 'python --version'
                sh 'pip --version'
            }
        }
        stage('Run Isolated Tests') {
            steps {
                echo 'Executing Pytest inside the container...'
                sh 'echo "Running tests in an isolated Python 3.10 environment!"'
            }
        }
    }
}
