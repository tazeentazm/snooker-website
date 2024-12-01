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
                sh 'npm install' // Installs project dependencies
            }
        }
        stage('Test') {
            steps {
                sh 'npm test' // Runs the test suite
            }
        }
        stage('Deploy') {
            steps {
                script {
                    // Add your deployment logic here
                    echo "Deploying the application..."
                }
            }
        }
    }
}
