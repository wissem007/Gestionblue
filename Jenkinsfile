node{
    
    def project = 'gestion' 
    def imageVersion = 'development' 
    def imageTag = "wissem007/${project}:${imageVersion}.${env.BUILD_NUMBER}" 
      environment {
        NEXUS_VERSION = "nexus3"
        NEXUS_PROTOCOL = "http"
        NEXUS_URL = "178.33.44.117:8081/"
        NEXUS_REPOSITORY = "maven-nexus-repo"
        NEXUS_CREDENTIAL_ID = "nexus-user-credentials"
    }
    
    stage("Git Clone"){
        git 'https://github.com/wissem007/Gestion.git'
    }
    
    stage("Maven Clean Build"){
        sh "mvn package -DskipTests=true"
       
    }
     


    
    
   
  

