pipeline {  
    environment {
        registry = "fabianborn/demo-app"
        registryCredential = 'docker-hub-cred'
    }  
    agent any
    stages {
        stage('Back-end') {
            agent {
                docker { image 'busybox' }
            }
            steps {
                sh 'ping -c 192.168.69.1'
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