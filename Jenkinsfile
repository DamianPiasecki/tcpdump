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
        sh '''
apt install gcc 
./configure '''
      }
    }
  }
}