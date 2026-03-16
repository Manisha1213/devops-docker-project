pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/Manisha1213/devops-docker-project.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t devops-webapp .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh 'docker run -d -p 8081:80 devops-webapp'
            }
        }

    }
}
