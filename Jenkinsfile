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
        stage('Step1') {
          steps {
            echo 'Test Message'
            fileExists 'RaysLocalFile.txt'
          }
        }
        stage('Step2') {
          steps {
            bat(script: 'TestBat.cmd', encoding: 'ascii', returnStatus: true, returnStdout: true)
          }
        }
      }
    }
  }
  environment {
    RAYSTART = '1'
  }
}