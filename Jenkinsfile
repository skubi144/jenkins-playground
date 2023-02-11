pipeline {
    agent {
        docker { image 'cypress/included:12.3.0' }
        }
    stages {
        stage('Test') {
            steps{
                sh 'echo Hello'
                sh 'cypress'
            }
        }
    }
}