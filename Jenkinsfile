pipeline {
    agent {
        label 'java-slave'
    }

    // environmental variables 
    environment {
        TODAYS_DAY = 'wednesday'
    }
    stages {
        stage('buildstage') {

            // when condition 
            when {
                environment name: 'TODAYS_DAY', value: 'thursday'
            }

            // step block
            steps {
                echo "executing pipeline for when example"
            }
        }
    }
}
