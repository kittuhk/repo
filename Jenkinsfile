pipeline {
    agent {
        label "jenkins-slave1"
    }
    environment {
        name = "REO"
        course = "Jenkins"
    }
    stages {
        stage ("First Stage"){
            steps {
                echo "Welcome ${name}"
                echo " Thanks for choosing ${course} course"
            }
        }
    }
}
