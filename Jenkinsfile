pipeline {

    agent any

    tools {
        nodejs 'node-12.8.0'
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

    }

}
