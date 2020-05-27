pipeline{
    agent any

    environment {
        DOCKER_REPO = 'faresyoussef'
        DOCKER_IMAGE = 'mutli-client'
    }

    stages{

        stage('Build'){
            steps{
                echo 'Building ...'
            }
        }

        stage('Test'){
            steps{
                echo 'Testing ...'
            }
        }

        stage('Dockerizing'){
            steps{
                echo("Creating Docker image for build: $BUILD_NUMBER")
                docker build -t ${DOCKER_REPO}/${DOCKER_IMAGE}:${BUILD_NUMBER}
            }
        }

    }

}