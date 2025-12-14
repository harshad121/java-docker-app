pipeline {
    agent any
    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/username/java-docker-devops.git'
            }
        }
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t java-docker-app .'
            }
        }
        stage('Run Container') {
            steps {
                sh 'docker run java-docker-app'
            }
        }
    }
}
