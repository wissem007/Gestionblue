pipeline {
  agent any
  
  tools {
        maven "Maven"
    }
  stages {
    stage('Clone code from Git') {
      steps {
        git(url: 'https://github.com/wissem007/Gestionblue.git', branch: 'master')
      }
    }

    stage('Maven Build') {
      steps {
        sh 'mvn -Dmaven.test.failure.igonre=true clean package'
      }
    }

    stage('') {
      steps {
        tool(name: 'maven', type: 'Maven')
      }
    }

  }
}
