pipeline {
  agent any
  stages {
    stage('Say Hello') {
      parallel {
        stage('Say Hello') {
          steps {
            echo 'Hello World'
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
}