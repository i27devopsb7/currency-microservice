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
