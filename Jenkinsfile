pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/YOUR_USERNAME/devops-docker-project.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t devops-webapp .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 8081:80 devops-webapp'
            }
        }

    }
}
=
