pipeline {
    agent {
        docker { image 'nginx:alpine' }
    }
    stages {
        stage('Deploy') {
            steps {
                script {
                    // Ensure the files you want to copy exist in the workspace
                    sh 'ls -l ${WORKSPACE}'
                    
                    // Copy files from Jenkins workspace to the Docker container
                    sh '''
                    cp -r ${WORKSPACE}/Jenkinsfile \
                          ${WORKSPACE}/README.md \
                          ${WORKSPACE}/background.jpg.jpg \
                          ${WORKSPACE}/index.html \
                          ${WORKSPACE}/script.js \
                          ${WORKSPACE}/style.css \
                          /usr/share/nginx/html/
                    '''
                }
            }
        }
    }
}
