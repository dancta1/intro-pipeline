pipeline {
  agent any
  stages {
    stage('Say Hello') {
      parallel {
        stage('Say Hello') {
          steps {
            echo 'Hello ${MY_NAME}!'
          }
        }
        stage('Say More Hello') {
          steps {
            echo 'Say More Hello'
            sh 'java -version'
          }
        }
      }
    }
  }
  environment {
    MY_NAME = 'Mary'
  }
}