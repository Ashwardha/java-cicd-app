pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/Ashwardha/java-cicd-app.git'
            }
        }

        stage('Build') {
            steps {
                sh 'echo Building application'
            }
        }

        stage('Test') {
            steps {
                sh 'echo Running tests'
            }
        }

        stage('SonarQube Analysis') {
            steps {
                sh 'echo Running SonarQube analysis'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'echo Building Docker image'
            }
        }

        stage('Deploy to Kubernetes') {
            steps {
                sh 'echo Deploying to Kubernetes'
            }
        }
    }
}
