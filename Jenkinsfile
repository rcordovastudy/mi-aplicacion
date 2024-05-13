pipeline {
    agent any
    
    environment {
        DOCKER_IMAGE = 'dockerfile:lastest'
    }
    
    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    // Construye la imagen Docker
                    sh "docker build -t $DOCKER_IMAGE ."
                }
            }
        }
    }
}
