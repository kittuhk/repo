pipeline {
    agent any
    stages{
        stage("Build"){
            steps{
                echo "Build stage"
            }
        }
        stage("Scan"){
            steps{
                echo "scan the code"
            }
        }
        stage("Dockerbuild"){
            steps{
                echo "build docker image"
            }
        }
        stage("deploy"){
            steps{
                echo "deploying "
            }
        }
    }
}
