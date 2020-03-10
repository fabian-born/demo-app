pipeline {  
    environment {
        registry = "fabianborn/demo-app"
        registryCredential = 'docker-hub-cred'
    }  
    agent { label 'master' }
    stages {
      stage('Building image') {
        steps{
          script {
            echo "build image"
            docker.build registry + ":$BUILD_NUMBER"
          }
        }
      }
    }
}