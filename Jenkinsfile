pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo $Name'
          }
        }
        stage('build2') {
          steps {
            sh 'echo "build2"'
          }
        }
      }
    }
    stage('Test') {
      steps {
        sh 'echo "Test"'
      }
    }
    stage('deployment') {
      steps {
        echo 'begin deployment'
      }
    }
  }
  environment {
    Name = 'hello world'
  }
}