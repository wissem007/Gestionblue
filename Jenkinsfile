pipeline {
  agent any
  stages {
    stage('docker') {
      parallel {
        stage('docker') {
          steps {
            sh 'docker ps'
          }
        }

        stage('intial') {
          steps {
            echo 'liste des container'
          }
        }

      }
    }

  }
}