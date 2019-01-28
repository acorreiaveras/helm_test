pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        script {
          sh 'echo ${USERNAME}'
          sh 'echo ${PASSWORD}'
        }

      }
    }
  }
  environment {
    USERNAME = 'credentials(\'smartcheck-credentials-username\')'
    PASSWORD = 'credentials(\'smartcheck-credentials-password\')'
  }
}