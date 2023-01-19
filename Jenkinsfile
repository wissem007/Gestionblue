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
        echo 'Docker run avec Succes '
      }
    }

    stage('login to dockerhub') {
      steps {
        sh 'echo $DOCKERHUB_CREDENTIALS_PSW | docker login -u $DOCKERHUB_CREDENTIALS_USR --password-stdin'
      }
    }

    stage('run docker image') {
      steps {
        sh 'docker push wissem007/nodejs:$BUILD_NUMBER'
      }
    }

  }
  environment {
    DOCKERHUB_CREDENTIALS = 'credentials(\'docker-hub-wissem\')'
  }
}