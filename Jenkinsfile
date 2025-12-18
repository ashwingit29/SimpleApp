pipeline {
  agent any
  stages {
    stage('Clone') {
      steps {
        git 'https://github.com/ashwingit29/SimpleApp.git'
      }
    }
    stage('Build Docker Image') {
      steps {
        sh 'docker build -t SimpleApp'
      }
    }
    stage('Test Container') {
      steps {
        sh 'docker run --rm SimpleApp'
      }
    }
  }
}

