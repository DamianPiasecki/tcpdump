pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          image 'ubuntu'
          args '-u 0'
        }

      }
      steps {
        sh '''apt update --y
apt install gcc --y
./configure '''
      }
    }
  }
}