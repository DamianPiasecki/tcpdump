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
        sh '''apt get update
apt get install gcc 
./configure '''
      }
    }
  }
}