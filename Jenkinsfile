pipeline {
    agent any
    environment {
        NVM_DIR = "/home/vagrant/.nvm"
        PATH = "${NVM_DIR}/versions/node/v21.7.3/bin:${env.PATH}"
    }
    stages {
        stage('build') {
            steps {
                sh "source ${NVM_DIR}/nvm.sh && npm install"
            }
        }
    }
}
