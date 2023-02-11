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
                sh 'apt-get install libgtk2.0-0 libgtk-3-0 libgbm-dev libnotify-dev libgconf-2-4 libnss3 libxss1 libasound2 libxtst6 xauth xvfb'
                sh './node_modules/.bin/cypress install --force'
                sh './node_modules/.bin/cypress run'
            }
        }
    }
}