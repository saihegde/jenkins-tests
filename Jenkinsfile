pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        sh '/opt/maven/bin/mvn deploy'
        input(message: 'Deploy to Sandbox', id: 'nexusCredentials', ok: 'username')
      }
    }
  }
}