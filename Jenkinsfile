pipeline {
    agent any

    environment {
        AWS_REGION = 'ap-south-1'
        ACCOUNT_ID = '026870878274'
    }

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/bennieshs54-collab/StreamingApp.git'
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
<<<<<<< HEAD
}
=======
}
>>>>>>> fc4e6665d40f4e25eef10e2cff2f75b8e2b62dd2
