pipeline {
    agent {
        label 'java-slave'
    }

    // environmental block
    environment {
        // key = value > ${key}
        name = "agnes"
        course = "Devops Engineer Program"

       // cloud = "GCP"
    }

    stages {
        stage ('FirstStage') {
            environment {
                cloud = "GCP"
            }
            steps {
                echo "Welcome ${name}"
                echo "You enrolled to ${course}"
                echo "You are certified in ${cloud} Cloud"
            }
        }

    }
}
