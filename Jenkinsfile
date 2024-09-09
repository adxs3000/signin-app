pipeline {
    agent {
        docker { image 'nginx:alpine' }
    }
    stages {
        stage('Deploy') {
            steps {
                // Example: Copy static files to the Nginx directory
                sh '''
                cp -r /home/xs475-arcdal/Task-1-Xenonstack-/* /usr/share/nginx/html/
                '''
            }
        }
    }
}
