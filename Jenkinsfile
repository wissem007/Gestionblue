stage('compile')
  agent {
    docker {
        image 'maven:3.6.0-jdk-8-alpine'
        args '-v /home.m2/repository:/root/.m2/repository'
           }
        }
    steps{
      sh 'mvn compile' 
}
