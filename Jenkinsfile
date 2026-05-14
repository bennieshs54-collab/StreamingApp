pipeline {
    agent any

    environment {
        AWS_REGION = 'ap-south-1'
        ACCOUNT_ID = 'YOUR_ACCOUNT_ID'
    }

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/YOUR_USERNAME/StreamingApp.git'
            }
        }

        stage('Build Backend') {
            steps {
                dir('backend') {
                    sh 'docker build -t backend .'
                }
            }
        }

        stage('Build Frontend') {
            steps {
                dir('frontend') {
                    sh 'docker build -t frontend .'
                }
            }
        }
    }
}
