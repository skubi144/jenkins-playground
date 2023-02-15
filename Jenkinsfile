pipeline {
    agent {
        docker { image 'cypress/included:12.5.1' }
        }
    stages {
        stage('Test') {
            steps{
                sh 'npm install'
                sh 'npm run e2e'
            }
        }
    }
}