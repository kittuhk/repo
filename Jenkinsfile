pipeline {
    agent {
        label "jenkins-slave1"
    }
    environment {
        name = "REO"
        course = "Jenkins"
        company = "sfty"
    }
    stages {
        stage ("First Stage"){
            steps {
                echo "Welcome ${name}"
                echo " Thanks for choosing ${course} course"
            }
        }
        stage (" Second Stage"){
            steps {
                echo " Welcome to ${company} world"
            }
        }
    }
}
