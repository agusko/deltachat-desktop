pipeline {
  agent {
    docker {
      image 'node:15.14.0-stretch'
    }

  }
  stages {
    stage('Build') {
      agent any
      steps {
        sh 'RUN apt-get update'
        sh '''
RUN npm install -g npm@7.8.0'''
        sh '''npm install
'''
        sh 'npm start build'
      }
    }

  }
}