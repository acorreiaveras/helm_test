pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        script {
          MY_USERNAME='echo $USERNAME'
          print MY_USERNAME
        }

      }
    }
  }
  environment {
    USERNAME = 'credentials(\'smartcheck-credentials-username\')'
    PASSWORD = 'credentials(\'smartcheck-credentials-password\')'
  }
}