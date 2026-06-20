pipeline {
    agent any
    
    // The new block! This creates a dropdown menu in the Jenkins UI
    parameters {
        choice(name: 'TEST_SUITE', choices: ['Smoke', 'Regression', 'Sanity'], description: 'Which test suite do you want to run?')
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Pulling code...'
            }
        }
        stage('Run Dynamic Tests') {
            steps {
                // Notice the ${params.TEST_SUITE} variable. 
                // Jenkins will replace this with whatever you select!
                echo "Initializing the ${params.TEST_SUITE} testing environment..."
                bat "echo Running ${params.TEST_SUITE} tests!"
            }
        }
    }
}
