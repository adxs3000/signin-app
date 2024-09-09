pipeline {
    agent {
        docker { image 'nginx:alpine' }
    }
    stages {
        stage('Build') {
            steps {
                sh 'node --version' // Note: node command is not available in nginx:alpine by default
            }
        }
    }
}
