pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage ('Build'){
            steps {
                echo "Build stage from feature Branch"
            }
        }
        stage ('Scans'){
            steps {
                echo "Scans stage from feature Branch"
            }
        }
        stage ('dockerbuild'){
            steps {
                echo "docker stage from feature Branch"
            }
        }
        stage ('deployment'){
            steps {
                echo "deploying from feature Branch"
            }
        }
    }
}
