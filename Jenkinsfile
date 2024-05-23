pipeline {
    agent any

    stages {
        stage('Debug') {
            steps {
                sh 'echo $PATH'
            }
        }
        stage('build') {
            steps {
                sh 'npm install -g npm'
            }
        }
    }
}
