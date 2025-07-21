pipeline {
    agent {
        label "jenkins-slave1"
    }
    environment {
        DEPLOY_TO = 'production'
    }
    stages{
        stage ("Build"){
            steps {
                echo "printing build stage"
                sh "hostname -i"
            }
        }
        stage ("prod"){
            when {
                allOf{
                    branch 'main'
                environment name : 'DEPLOY_TO', value : 'production'
                }
            }
            steps{
                echo "Deploy to production"
            }
        }
    }
}
