pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building the application"
            }
        }
    }
    post {
        success {
            // code , will trigger only if the pipeline is succesfulle
            echo "Post ==================> Success block is triggered"
        }
        failure {
            // will trigger only if the pipeline is failed
            echo "Post ==================> Failure block is triggered"
        }
        always {
            // will trigger this block, irrespective of failure or sucess
            echo "Post ==================> always block is triggered"
        }
    }
}
