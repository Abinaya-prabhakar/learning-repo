pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Abinaya-prabhakar/learning-repo.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    sh 'docker build -t day20-app .'
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    sh 'docker run day20-app'
                }
            }
        }
    }
}

