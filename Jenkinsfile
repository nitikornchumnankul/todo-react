pipeline {
  agent any
  stages {

    stage('Check Stages') {
      steps {
        echo 'The next stage to npm install'
        cd "%WORKSPACE%"
        sh 'pwd'
      }
    }

    stage('install') {
      steps {
        sh 'cd todos'
        sh 'pwd'
        sh 'npm install'
      }
    }

    stage('build') {
      steps {
        sh 'npm run build'
      }
    }

    stage('docker image') {
      steps {
        sh 'docker build -t react-todo .'
      }
    }

  }
}
