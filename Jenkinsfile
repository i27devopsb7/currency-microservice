pipeline {
    agent {
        label 'java-slave'
    }

    // environmental block
    environment {
        // key = value > ${key}
        name = "agnes"
        course = "Devops Engineer Program"
        SONAR_URL = "sonar.hsbc.com"
       // cloud = "GCP"

        // the below is wrong
       //SONAR_TOKEN = "123456789"

       SONAR_CREDS  = credentials('sonar_creds')
    }

    stages { //highes precendence
        stage ('FirstStage') {
            environment {
                cloud = "GCP"
                name = "Mahesh babu"
            }
            steps {
                echo "Welcome ${name}"
                echo "You enrolled to ${course}"
                echo "You are certified in ${cloud} Cloud"
            }
        }
        stage ('SecondStage'){
            environment{
                admission_no = "12345"
            }
            steps {
                echo "Second stage: Welcome ${name}"
                echo "Second stage: You enrolled to ${course}"
                echo "My admission number is ${admission_no}"
                echo "Printing my token: ${SONAR_CREDS}"
            }
        }

    }
}

