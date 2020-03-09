pipeline {
    agent none
    stages {
        stage('Back-end') {
            agent {
                docker { }
            }
            steps {
                sh "docker login -u fabianborn -p ${env.DOCKER_HUB_PASSWORD} "
        }
    }
}