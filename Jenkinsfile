/Here is the parallel pipeline
pipeline {
    agent any
    stages {
        stage ("Build"){
            steps {
                echo "Building the application"
            }
        }
        stage ("scans"){
            parallel{
                stage ("sonar scan"){
            steps{
                echo "sonar scan is executing"
                sleep 15
            }
        }
        stage ("Fortifyscan"){
            steps{
                echo "fortifyscan is executing"
                sleep 15
            }
        }
        stage ("Prismascan"){
            steps{
                echo "prismascan is executing"
                sleep 15
            }
        }
        
        }
    }
}}
