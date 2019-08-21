pipeline {
  agent {
    docker {
      image 'golang'
    }

  }
  stages {
    stage('Check') {
      steps {
        sh 'go get -v -t -d ./...'
      }
    }
    stage('Build') {
      steps {
        sh 'go build -v .'
      }
    }
  }
}