pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        node {
          label '15.14.0-stretch'
        }

      }
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