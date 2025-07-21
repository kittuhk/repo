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
                expression {BRANCH_NAME ==~ /(main|deploy)/ }
            }
            steps {
                echo "executing pipeline for when example"
            }
        }
