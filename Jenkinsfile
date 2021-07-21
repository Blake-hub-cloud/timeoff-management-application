pipeline {

    agent any

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

    }

}
