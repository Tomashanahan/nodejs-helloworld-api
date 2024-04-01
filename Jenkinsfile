pipeline {
    agent any
    stages {
        stage('Installing dependencies') {
            steps {
                sh 'npm install'
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