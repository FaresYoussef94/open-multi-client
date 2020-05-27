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
                echo 'Creating the docker image ... ${BUILD_NUMBER}'
                sh 'ls'
            }
        }

    }

}