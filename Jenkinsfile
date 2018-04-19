pipeline {
  agent {
    docker {
      image 'golang:1.10.1-alpine'
      label 'docker-cloud'
    }
    
  }
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
            sh 'go version'
          }
        }
      }
    }
  }
}