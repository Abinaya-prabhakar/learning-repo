// Jenkinsfile
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
                    sh 'docker build -t hello-abinaya .'
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    sh 'docker run hello-abinaya'
                }
            }
        }
