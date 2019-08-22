pipeline {
  agent {
    docker {
      args '-p 3030:3030'
      image 'node:6-alpine'
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