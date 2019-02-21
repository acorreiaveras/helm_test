pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        script {
          sh'echo $env:smartcheck-username'
        }

      }
    }
  }
  environment {
    USERNAME = 'credentials(\'smartcheck-credentials-username\')'
    PASSWORD = 'credentials(\'smartcheck-credentials-password\')'
  }
}