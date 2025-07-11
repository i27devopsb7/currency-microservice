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
        stage ('Scans') {
            parallel {
                stage ('SonarScans') {
                    steps {
                        echo "Sonar scan is executing"
                        sleep 15
                    }
                }
                stage ('FortifyScans') {
                    steps {
                        echo "Fortify scan is executing"
                        sleep 15
                    }
                }
                stage ('PrismaScans') {
                    steps {
                        echo "Prisma scan is executing"
                        sleep 15
                    }
                }
            }
        }
        stage ('DeployToDev') {
            steps {
                echo "Deploying to dev environment"
                // k8s code
            }
        }
        stage ('DeployToTest') {
            steps {
                echo "Deploying to test environment"
            }
        }
        stage ('DeployToStage') {
            steps {
                echo "Deploying to Stage environment"
            }
        }
        stage ('DeployToProd') {
            steps {
                echo "Deploying to Prod environment"
            }
        }
    }
}
