pipeline {
    agent {
        label 'java-slave'
    }

    // environmental block
    environment {
        // key = value > ${key}
        name = "Siva"
        course = "Devops Engineer Program"
    }

    stages {
        stage ('FirstStage') {
            steps {
                echo "Welcome ${name}"
                echo "You enrolled to ${course}"
            }
        }

    }
}
