pipeline {  
    environment {
        registry = "fabianborn/demo-app"
        registryCredential = 'docker-hub-cred'
    }  
    agent any
    stages {
        stage('Back-end') {
            agent {
                docker { image 'maven:3-alpine' }
            }
            steps {
                sh 'mvn --version'
            }
        }
    
      stage('Building image') {
        steps{
          script {
            echo "build image"
          }
        }
      }
    }
}