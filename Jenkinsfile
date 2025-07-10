pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage ('Build'){
            steps {
                echo "*********** Building the application **************"
            }
        }
        stage ('Sonar'){
            steps {
                echo "*********** Performing sonar scans ***********"
            }
        }
        stage ('DockerBuild'){
            steps {
                echo "*********** Building docker image ***********"
            }
        }
        stage ('DeployToDevEnv'){
            steps {
                echo "*********** Deploying to dev environment ***********"
            }
        }
        stage ('DeployToTestEnv'){
            steps {
                echo "*********** Deploying to test environment ***********"
            }
        }
        stage ('DeployToStageEnv'){
            when {
                branch 'release-*'
            }
            steps {
                echo "*********** Deploying to stage environment ***********"
            }
        }
        stage ('DeployToProdEnv'){
            when { //v1.0.0
                tag pattern: "v\\d{1,2}.\\d{1,2}.\\d{1,2}"
            }
            steps {
                echo "*********** Deploying to Prod environment ***********"
            }
        }
    }
}
