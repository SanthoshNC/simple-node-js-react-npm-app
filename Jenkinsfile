pipeline {
    agent {
        docker {
            image 'node:current-slim'
            args '-p 3000:3000'
        }
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm cache clean -force'
                sh 'npm install' 
            }
        }
    }
}

