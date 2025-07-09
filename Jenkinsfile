pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage ('Build'){
            steps {
                echo "Building the application"
            }
        }
        stage ('Scans'){
            steps {
                echo "Performing sonar scans"
            }
        }
        stage ('dockerbuild'){
            steps {
                echo "Implementing docker build"
            }
        }
        stage ('devenv'){
            steps {
                echo "deploying to dev env"
            }
        }
        stage ('stageenv'){
            steps {
                echo "deploying to stage env"
            }
        }
        stage ('prodenv'){
            steps {
                echo "deploying to prod env"
            }
        }
    }
}
