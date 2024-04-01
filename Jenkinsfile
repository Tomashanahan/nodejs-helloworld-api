pipeline {
    agent any
    stages {
        stage('Installing dependencies') {
            steps {
                // sh 'npm install'
                sh '/home/jenkins/.nvm/versions/node/<version>/bin/npm install'
                echo 'Installing dependencies..'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
                echo 'Testing..'
            }
        }
    }
}