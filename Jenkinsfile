pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        sh 'cd java'
      }
    }
    stage('Build') {
      steps {
        sh 'javac Hello.java'
      }
    }
    stage('Compile') {
      steps {
        sh 'java Hello'
      }
    }
    stage('Done') {
      steps {
        echo 'Done'
      }
    }
  }
}