//here is the parallel block code
pipeline {
    agent any
    stages {
        stage ("Build"){
            steps {
                echo " Building the application "
            }
        }
        stage ("scans"){
            parallel{
                stage("Sonarscans"){
                    steps{
                        echo "Sonarscan is executing"
                        sleep 15
                    }
                }
                stage("Fortifyscan"){
                    steps{
                        echo "Fortifyscan is executing"
                        sleep 15
                    }
                }
                stage("Prismascan"){
                    steps{
                        echo "Prismascan is eexecuting"
                        sleep 15
                    }
                }
            }
        }
    }
}
