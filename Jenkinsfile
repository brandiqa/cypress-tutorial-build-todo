pipeline {
    agent {
        docker {
            image '10.16.3-buster-slim'
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
