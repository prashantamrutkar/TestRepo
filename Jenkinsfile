pipeline {
    agent any
    environment {
        PREVIOUS_BUILD_RESULT = 'currentBuild.getPreviousBuild().getResult().toString()'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'    
                echo '${env.PREVIOUS_BUILD_RESULT}'
      echo '${PREVIOUS_BUILD_RESULT}'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
