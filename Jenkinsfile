 node {   
    stage("Checkout") {
        echo "hallo Jenkins!"
    }                   
    stage("build docker") {
    
        container('docker') {
            withCredentials([[$class: 'UsernamePasswordMultiBinding',
                credentialsId: 'docker-hub-cred',
                usernameVariable: 'DOCKER_HUB_USER',
                passwordVariable: 'DOCKER_HUB_PASSWORD']]) {
                
                    sh "docker login -u ${env.DOCKER_HUB_USER} -p ${env.DOCKER_HUB_PASSWORD}"
            }
        }
    }
}
