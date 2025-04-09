pipeline {
    agent any

    environment {
        APP_NAME = "my-node-app"
        IMAGE_TAG = "my-node-app:latest"
    }

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t $IMAGE_TAG .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker rm -f $APP_NAME || true'
                sh 'docker run -d --name $APP_NAME -p 3000:3000 $IMAGE_TAG'
            }
        }
    }
}
