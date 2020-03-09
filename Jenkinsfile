node('node'){
    stage("Checkout") {
        echo "hallo Jenkins!"
    }
    stage("build docker") {    
        withCredentials([[$class: 'UsernamePasswordMultiBinding',
            credentialsId: 'docker-hub-cred',
            usernameVariable: 'DOCKER_HUB_USER',
            passwordVariable: 'DOCKER_HUB_PASSWORD']]) {
                        
        }
    }
}