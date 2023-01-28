pipeline {
    agent any

    stages {
        stage ('Build Docker Image') {
            script {
                dockerapp = docker.build("hernanisoares/kube-news:${env.BUILD_ID}", "-f ./src/Dockerfile ./src")
            }

        }
    }
}