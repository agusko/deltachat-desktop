pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        sh 'apt-get update'
        sh 'apt-get install -y npm'
        sh 'npm install -g npm@7.8.0'
        sh 'npm install'
        sh 'npm start build'
      }
    }

  }
}