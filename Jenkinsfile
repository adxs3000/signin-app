Jenkinsfile (Declarative Pipeline)
/* Requires the Docker Pipeline plugin */
pipeline { 
    agent { docker { image 'nginx:alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'node --version'
            }
        }
    }
}
