pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          image 'ubuntu'
        }

      }
      steps {
        sh '''apt update
apt install gcc 
./configure '''
      }
    }
  }
}