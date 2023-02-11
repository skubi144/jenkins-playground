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
            steps {
                echo 'Testing.....'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying.......'
            }
        }
    }
}