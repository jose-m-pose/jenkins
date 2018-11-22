pipeline {
  agent any
  stages {
    stage('Paso1') {
      steps {
        sh 'git clone https://github.com/CGD14/PruebaDeEdu2.git'
      }
    }
    stage('paso 2') {
      steps {
        echo 'aqui en paso 2'
      }
    }
    stage('paso 3') {
      parallel {
        stage('paso 3') {
          steps {
            sh 'ls -lrt'
          }
        }
        stage('paso 3.3') {
          steps {
            echo 'ejeje'
          }
        }
      }
    }
  }
}