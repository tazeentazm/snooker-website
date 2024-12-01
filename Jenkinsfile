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
                    // Using an explicit closure
                    { 
                        sh 'npm install'
                    }.call()
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    // Using an explicit closure
                    { 
                        sh 'npm test'
                    }.call()
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

