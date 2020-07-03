pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-u 0:0' 
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
