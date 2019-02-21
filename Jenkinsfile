pipeline {
  agent any
  stages {
    stage('print credentials') {
      steps {
        script {

          withCredentials([usernamePassword(credentialsId: 'smartcheck-credentials',
          usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {
            sh 'echo $PASSWORD'
            echo "${env.USERNAME}"
          }

        }

      }
    }
  }
  environment {
    USERNAME = 'credentials(\'smartcheck-credentials-username\')'
    PASSWORD = 'credentials(\'smartcheck-credentials-password\')'
  }
}