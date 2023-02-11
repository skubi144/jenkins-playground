pipeline {
    agent {
        docker { image 'node:16.13.1-alpine ' }
        }
    stages {
        stage('Test') {
            steps{
                sh 'echo Hello'
                sh 'npm i'
                sh 'npm run cypress:ci'
            }
        }
    }
}