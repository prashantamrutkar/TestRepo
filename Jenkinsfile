pipeline {
    agent any
    environment {
        PREVIOUS_BUILD_RESULT = 'currentBuild.getPreviousBuild().getResult()'
    }
    withEnv(["PREVIOUS_BUILD_RESULT=currentBuild.getPreviousBuild().getResult()"]) {
      echo '${env.PREVIOUS_BUILD_RESULT}'
      echo '${PREVIOUS_BUILD_RESULT}'
      }
}

    stages {
        stage('Build') {
            steps {
                echo 'Building..'                
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
