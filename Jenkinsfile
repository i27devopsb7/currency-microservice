pipeline {
    agent {
        label 'java-slave'
    }

//     tools {

//     }

//     environment {
// // ${ENV_NAME}
//     }

    parametes {
        string(name: 'APPLICATION_NAME', description: 'Enter your application name', defaultValue: 'i27App')
        booleanParam(name: 'RUN_TESTS', description: 'Woulr you like to run tests ?', defaultValue: true)
        choice(name: 'ENV', description: 'Which env should i be deploying ?', choices: ['dev', 'test', 'prod'])
        password(name: 'PASSWORD', description: 'Enter a password', defaultValue: 'SECRET')
    }

    stages {
        stage ('parametesExample'){
            steps {
                //code 
                echo "My application name is : ${params.APPLICATION_NAME}"
                echo "Are testing running ? ${params.RUN_TESTS}"
                echo "Deploying to *** ${params.ENV} ****"
                echo "Password Entered is: ${params.PASSWORD}"
            }
        }
    }
}
