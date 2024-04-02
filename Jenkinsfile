pipeline {
    agent any
    tools {
        nodejs "NodeJS"
    }
    stages {
        stage('Installing dependencies') {
            steps {
                sh 'npm install'
                echo '❌'
                sh "npm --version"
                echo '❌'
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