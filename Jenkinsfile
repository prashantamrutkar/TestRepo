pipeline {
    agent any
    environment {
        PREVIOUS_BUILD_RESULT = ${currentBuild.getPreviousBuild().getResult()?}
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo 'PREVIOUS_BUILD_RESULT : ${env.PREVIOUS_BUILD_RESULT}'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                echo 'PREVIOUS_BUILD_RESULT : ${env.PREVIOUS_BUILD_RESULT}'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                echo 'PREVIOUS_BUILD_RESULT : ${PREVIOUS_BUILD_RESULT}'
            }
        }
    }
}
