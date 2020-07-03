pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000' 
        }
    }
    environment { 
        HOME='/home/node'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install --unsafe-perm=true --allow-root'
                sh 'npm install' 
            }
        }
    }
}
