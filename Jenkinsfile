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
            echo 'Test Message'
            fileExists 'RaysLocalFile.txt'
          }
        }
      }
    }
  }
  environment {
    RAYSTART = '1'
  }
}