pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      agent any
      steps {
        sh '''
RUN npm install -g npm@7.8.0'''
        sh '''npm install
'''
        sh 'npm start build'
      }
    }

  }
}