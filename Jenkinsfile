pipeline {
  agent {
    docker {
      image 'node:15.14.0-stretch'
      args '-p 3000:3000'
    }

  }
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