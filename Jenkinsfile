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
        stage('error') {
          steps {
            sh 'set'
          }
        }
      }
    }
  }
  environment {
    RAYSTART = '1'
  }
}