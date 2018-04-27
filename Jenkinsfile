pipeline {
  agent any
  stages {
    stage('Compile') {
      parallel {
        stage('Compile') {
          steps {
            echo 'Hi There'
          }
        }
        stage('') {
          steps {
            sh 'env'
          }
        }
      }
    }
  }
  environment {
    RAYSTART = '1'
  }
}