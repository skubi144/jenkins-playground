pipeline {
    agent {
        docker { image 'node:16.13.1-alpine' }
        }
    stages {
        stage('Test') {
            steps{
                sh 'echo Hello'
                sh 'ls'
                sh 'npm install'
                sh 'ls node_modules'
                sh './node_modules/.bin/cypress install --force'
                sh './node_modules/.bin/cypress run'
            }
        }
    }
}