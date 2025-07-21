pipeline {
    agent{
        label "jenkins-slave1"
    }
    environment {
        TODAYS_DAY = " Monday "
    }
    stages{
        stage("Build Stage"){
            when {
                environment name : 'TODAYS_DAY', value : ' Monday '
            }
            steps {
                echo "executing pipeline for when example"
            }
        }
    }
}

