// Here i am declaring environment block under the stage level
//i will change the name in the stage block it wil consider stage block for high preference 
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
            environment {
                name = " Kittu "
                course = " Maven "
            }   
            steps {
                echo "Welcome ${name}"
                echo " Thanks for choosing ${course} course"
                echo " Welcome to ${company}"
            }
        }
        stage (" Second Stage"){
            steps {
                echo " Welcome to ${company} world"
            }
        }
    }
}
