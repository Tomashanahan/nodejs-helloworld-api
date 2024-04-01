pipeline {
    agent any
    stages {
        stage('Installing dependencies') {
            steps {
                bat 'npm install'
                echo 'Installing dependencies..'
            }
        }
        stage('Test') {
            steps {
                bat 'npm test'
                echo 'Testing..'
            }
        }
    }
}