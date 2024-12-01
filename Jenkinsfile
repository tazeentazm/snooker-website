pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/tazeentazm/snooker-website.git'
            }
        }
        stage('Install') {
            steps {
                // Run npm install
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                // Run npm test
                sh 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                script {
                    // Add deployment logic here
                    echo "Deploying the application..."
                }
            }
        }
    }
}
