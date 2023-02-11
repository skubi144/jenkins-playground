pipeline {
    agent {
            docker { image 'node:16.13.1-alpine' }
    }
    stages {
        stage('Build') {
            steps {
                sh 'ls'
                echo 'Building.... from git'
            }
        }
        stage('Test') {
            steps{
                sh 'npm i'
                sh 'npm run cypress:ci'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying.......'
            }
        }
    }
}