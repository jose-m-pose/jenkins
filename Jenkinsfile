pipeline {
  agent any
  stages {
    stage('Paso1') {
      steps {
        sh 'cd /home/jpr'
        sh '''

git clone https://github.com/CGD14/PruebaDeEdu2.git'''
        sh 'ls -lrt'
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