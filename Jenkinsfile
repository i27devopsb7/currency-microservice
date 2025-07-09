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
        stage ('SecondStage'){
            steps {
                echo "Second stage: Welcome ${name}"
                echo "Second stage: You enrolled to ${course}"
                echo "Second stage: You are certified in ${cloud} Cloud"
            }
        }

    }
}
