pipeline {
  agent any
     docker {
            image 'maven:3.8.1-adoptopenjdk-11' 
            args '-v /root/.m2:/root/.m2' 
        }
  
    stage('build') {
             steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
