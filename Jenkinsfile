pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'npm cache clean -force'
                sh 'npm install' 
            }
        }
    }
}

