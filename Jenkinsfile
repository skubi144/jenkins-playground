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
            agent {
                    docker { image 'cypress/included:12.3.0' }
            }
            steps{
                sh 'cypress'
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