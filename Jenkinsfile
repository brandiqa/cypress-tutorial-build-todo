pipeline {
    agent {
        docker {
            image 'node:lts-alpine'
            args '-p 3030:3030'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
    }
}
