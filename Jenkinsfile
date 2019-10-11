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
        sh 'apt -y update'
        sh 'apt -y install gcc make libpcap-dev'
        sh './configure'
      }
    }
  }
}