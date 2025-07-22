pipeline {
    agent any
    stages {
        stage("Build"){
            steps{
                echo " Building post block pipeline "
            }
        }
    }
    post {
        success{          //code will trigger only the pipeline is successful
            echo "print pipeline is success"
        }
        failure {        //code will trigger only the pipeline is failure
            echo "print pipeline is failure"
        }
        always[           //will trigger this block, irrespective of succuss or failure 
                        // mail wil also trigger here
            echo "always block is triggered"
        ]
    }
}
