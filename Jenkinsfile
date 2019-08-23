pipeline {
    agent {
        docker {
            image 'cypress/base:10'
            args '-p 3030:3030'
        }
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'npx cypress verify'
                sh 'npm test'
            }
         }
    }
}
