pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'ls'
                echo 'Building.... from git'
            }
        }
        stage('Test') {
            agent {
                docker { image 'node:16.13.1-alpine' }
            }
            steps{
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