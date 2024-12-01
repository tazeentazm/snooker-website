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
                script {
                    // Corrected syntax
                    sh 'npm install'
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    // Corrected syntax
                    sh 'npm test'
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    // Add your deployment logic here
                }
            }
        }
    }
}
