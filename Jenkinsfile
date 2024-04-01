pipeline {
    agent any
    stages {
        stage('Installing dependencies') {
            steps {
                // sh 'npm install'
                sh '/var/lib/jenkins/.nvm/versions/node/v20.11.0/bin/npm install'
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