pipeline {
    agent {
        docker { image 'nginx:alpine' }
    }
    stages {
        stage('Deploy') {
            steps {
                // Example: Copy static files to the Nginx directory
                sh '''
                cp -r github.com/adxs3000/signin-app.git * /usr/share/nginx/html/
                '''
            }
        }
    }
}
