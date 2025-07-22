pipeline {
    agent any
    stages {
        stage ("Build"){
            steps {
                echo " Building the application "
            }
        }
        stage ("scans"){
            parallel{ //here below the stage we can add parallel block 
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
        stage("DeployToDev"){
            steps{
                echo "Deploying to dev environment"
            }
        }
        stage("DeployToTest"){
            steps{
                echo "Deploying to test environment"
            }
        }
        stage("DeployToStage"){
            steps{
                echo "Deploying to stage environment"
            }
        }
        stage("DeployToProd"){
            options{
                timeout(time:300, units:'SECONDS')
            }
            input{
                message "Doing Prod Deployments ?"
                ok "yes"
                submitter "hari,mani" //who would be having access to approve
            }
            steps{
                echo "Deploying to prod enviroment"
                //timeout(time:300 ,units:'SECONDS')
                      //input message: "Doing Prod Deployments ?",ok:"yes",submitter: "hari,mani"
            }
        }
        
    }
}
