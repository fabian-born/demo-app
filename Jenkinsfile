node {
    checkout scm
    def customImage = docker.build("demo-app:${env.BUILD_ID}")
    customImage.push()
    
}
