pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('docker') {
      steps {
        sh 'docker run hello-word'
      }
    }

    stage('scrip') {
      steps {
        echo 'test'
      }
    }

  }
}