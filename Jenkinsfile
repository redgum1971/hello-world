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
        stage('Stage1_BasicTest') {
          steps {
            echo 'Test Message'
            fileExists 'RaysLocalFile.txt'
          }
        }
        stage('Stage2_BatFile') {
          steps {
            // bat(script: 'TestBat.cmd', encoding: 'ascii', returnStatus: true, returnStdout: true)
            echo 'In place of the windows bat file'
          }
        }
      }
    }
    stage('Test') {
      steps {
        echo 'Test Step'
      }
    }
  }
  environment {
    RAYSTART = '1'
  }
}