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
                docker "cypress/included:12.3.0"
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