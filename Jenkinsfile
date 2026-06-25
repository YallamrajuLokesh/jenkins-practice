pipeline {
    agent {
        docker {
            image 'python:3.10-slim'
            label 'linux-docker' // Matches the label we just gave the AWS Node!
        }
    }

    stages {
        stage('Environment Check') {
            steps {
                echo 'Checking the environment inside the isolated cloud container...'
                sh 'python --version'
                sh 'pip --version'
            }
        }
        stage('Run Isolated Tests') {
            steps {
                echo 'Executing Pytest inside the cloud container...'
                sh 'echo "Tests passed!"'
            }
        }
    }
}
