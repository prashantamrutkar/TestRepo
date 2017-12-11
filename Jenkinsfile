pipeline {
    agent any
    environment {
        PREVIOUS_BUILD_RESULT = 'true'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo 'PREVIOUS_BUILD_RESULT : ${PREVIOUS_BUILD_RESULT}'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                echo 'PREVIOUS_BUILD_RESULT : ${PREVIOUS_BUILD_RESULT}'
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
