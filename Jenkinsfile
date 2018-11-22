pipeline {
  agent {
    docker {
      image 'maven:3.3.3'
    }

  }
  stages {
    stage('build') {
      steps {
        retry(count: 3) {
          sh 'mvn --version'
        }

      }
    }
  }
}