pipeline {
    agent any
    tools { nodejs "NodeJS" }
    stages {
        stage('Build') { 
            steps {
                sh 'rm -rf node_modules'
                sh 'npm install' 
            }
        }
    }
}
