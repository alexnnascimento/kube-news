pipeline {
    agent any

    stages {
        
        stages ('Build Docker Image') {
            steps {
                scrip {
                    dockerapp = docker.build("alexnnascimento/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }

    }


}