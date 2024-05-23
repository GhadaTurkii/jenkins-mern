pipeline {
    agent any

    stages {
        stage('Install npm') {
            steps {
                nodejs(nodeJSInstallationName: 'Node 6.x', configId: '<config-file-provider-id>') {
                    sh 'npm install -g npm'
                }
            }
        }
    }
}
