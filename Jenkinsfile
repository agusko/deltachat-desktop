pipeline {
  agent any
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