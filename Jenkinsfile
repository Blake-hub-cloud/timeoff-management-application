pipeline {

    agent any

    environment {
        DOCKER_IMAGE_NAME = "$application_name-application"
    }


    tools {
        nodejs '12.18.0'
    }

    stages {

        stage ('Checkout') {
            steps {
                
                sh ('ls -l')
            }
        }

        stage ('Npm Install') {
            steps {
                
                sh ('npm install')
            }
        }


        stage ('Building Docker Image') {
            steps {
                
                sh ('docker build --no-cache . -t $DOCKER_IMAGE_NAME:$BUILD_NUMBER -f Dockerfile.Optional')  
            }
        }

    }

}