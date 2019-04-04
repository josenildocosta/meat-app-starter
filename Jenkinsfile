pipeline {
  agent {
    docker {
      image 'maven'
    }

  }
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
  }
}