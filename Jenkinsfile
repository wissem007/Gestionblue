pipeline {
  agent any {
    docker {
      image 'node:lts-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('bluid') {
      steps {
        sh 'npm install'
      }
    }

  }
}
