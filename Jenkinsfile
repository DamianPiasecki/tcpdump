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
        sh '''-u 0
apt update
apt install gcc 
./configure '''
      }
    }
  }
}