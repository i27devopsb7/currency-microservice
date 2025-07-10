pipeline {
    agent {
        label 'java-slave'
    }

    // environmental variables 
    environment {
        TODAYS_DAY = 'thursday'
    }

    stages {
        stage('buildstage') {

            // when condition 
            // when {
            //     environment name: 'TODAYS_DAY', value: 'thursday'
            // }
            when {
                expression { BRANCH_NAME ==~ /(prod|hotfix)/ }
            }
            // step block
            steps {
                echo "executing pipeline for when example"
            }
        }
    }
}
