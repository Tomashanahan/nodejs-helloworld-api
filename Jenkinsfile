pipeline {
    agent any
    tools {
        nodejs "NodeJS"
    }
    stages {
        stage('Installing dependencies') {
            steps {
                echo '📦 Installing dependencies.. 📦'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo '🧪 Testing.. 🧪'
                sh 'npm test'
            }
        }
    }
}