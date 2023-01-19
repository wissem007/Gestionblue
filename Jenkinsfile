pipeline {
  agent any
  stages {
    stage('Git check Out') {
      steps {
        git(url: 'https://github.com/wissem007/nodejs-demo.git', branch: 'master')
        echo 'Sucess pour le clonage github'
      }
    }

    stage('Build docker imag') {
      steps {
        sh 'docker build -t wissem007/nodeapp:$BUILD_NUMBER .'
      }
    }

  }
}