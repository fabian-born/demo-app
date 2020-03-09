pipeline {  
    environment {
        registry = "fabianborn/webapp"
        registryCredential = 'docker-hub-cred'
    }  
    agent any
    stages {
      stage('Building image') {
        steps{
          script {
            echo "build image"
          }
        }
      }
    }
}