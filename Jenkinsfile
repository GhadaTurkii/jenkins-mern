pipeline {
    agent any

    stages {
        stage('Install npm') {
            steps {
                script {
                    // Check if npm is installed
                    def npmVersion = sh(script: 'npm -v', returnStdout: true).trim()
                    if (npmVersion == '') {
                        // If npm is not installed, install it
                        sh 'curl -fsSL https://npmjs.com/install.sh | sh'
                    } else {
                        echo "npm is already installed (version: ${npmVersion})"
                    }
                }
            }
        }
        stage('Build') {
            steps {
                sh 'npm install' // Example npm command, adjust as needed
            }
        }
    }
}
