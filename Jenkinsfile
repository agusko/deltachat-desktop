pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        sh 'npm install'
        sh 'npm run build'
      }
    }

  }
}