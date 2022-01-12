pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        echo 'The next stage to npm install'
        sh 'bat npm install'
        sh 'apt install npm'
      }
    }

  }
}