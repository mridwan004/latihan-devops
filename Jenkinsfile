pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/username/repo.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t aplikasi-pertamaku .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 8080:8080 aplikasi-pertamaku'
            }
        }
    }
}