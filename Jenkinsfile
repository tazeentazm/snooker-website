pipeline {
    agent any
    stages {
        stage('Clone Code') {
            steps {
                git branch: 'main', url: 'https://github.com/tazeentazm/snooker-website.git'
            }
        }
        stage('Build') {
            steps {
                echo 'No build required for static sites'
            }
        }
        stage('Deploy') {
            steps {
                sh '''
                # Deploy locally or via SSH
                scp -r * user@remote-server:/var/www/static-site
                echo "Deployment complete!"
                '''
            }
        }
    }
}
