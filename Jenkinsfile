pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000' 
        }
    }
    environment { 
        HOME='/tmp'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm config set cache /tmp'
                sh 'npm install' 
            }
        }
    }
}
