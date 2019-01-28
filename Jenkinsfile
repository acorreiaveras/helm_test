pipeline {
  agent any
  stages {
    stage('') {
      steps {
        script {
          sh 'echo ${env.USERNAME}'
          sh 'echo ${env.PASSWORD}'
        }

      }
    }
  }
  environment {
    USERNAME = 'credentials(\'smartcheck-credentials-username\')'
    PASSWORD = 'credentials(\'smartcheck-credentials-password\')'
  }
}