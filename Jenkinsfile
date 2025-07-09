pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage ('Build'){
            steps {
                echo "Build stage from main Branch"
            }
        }
        stage ('Scans'){
            steps {
                echo "Scans stage from main Branch"
            }
        }
        stage ('dockerbuild'){
            steps {
                echo "docker stage from main Branch"
            }
        }
        stage ('deployment'){
            steps {
                echo "deploying from main Branch"
            }
        }
    }
}
