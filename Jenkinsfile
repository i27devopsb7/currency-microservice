pipeline{
    agent {
        label 'java-slave'
    }

    environment {
        DEPLOY_TO = 'production'
    }

    stages {
        stage ('DeploytoDev'){
            steps {
                echo "Deploying to dev env"
            }
        }
        stage ('ProdDeploy')
        {
            when {
                anyOf {
                    branch 'production'
                    environment name: 'DEPLOY_TO', value: 'production'
                }
            }
            steps {
                echo "*********** Deploying to production ***********"
            }
        }
    }
}
