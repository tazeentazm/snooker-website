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
                    // Using explicit closure syntax
                    { it ->
                        sh 'npm install'
                    }.call()
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    // Using explicit closure syntax
                    { it ->
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

