stage('compile')
  agent {
    docker {
        image 'maven:3.6-jdk-8-alpine'
        args '-v /root/.m2:/root/.m2' 
    }
    }
    steps{
      sh 'mvn compile' 
    }
