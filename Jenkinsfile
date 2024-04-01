pipeline {
    agent any
    stages {
        stage('Installing dependencies') {
            steps {
                // sh 'npm install'
                sh '''
                    export NVM_DIR="$HOME/.nvm"
                    [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
                    npm install
                    '''
                echo 'Installing dependencies..'
            }
        }
        // stage('Test') {
        //     steps {
        //         sh 'npm test'
        //         echo 'Testing..'
        //     }
        // }
    }
}