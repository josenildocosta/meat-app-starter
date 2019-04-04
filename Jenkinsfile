pipeline {
  agent none
  stages {
    stage('Client') {
      agent {
        docker {
          image 'node:6'
          args '-u 0:0'
        }

      }
      steps {
        sh 'npm install'
      }
    }
    stage('Deploy') {
      agent {
        docker {
          image 'node:6'
          args '-u 0:0'
        }

      }
      steps {
        sh 'npm start'
      }
    }
  }
}