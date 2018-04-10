pipeline {
  agent any
  stages {
    stage('Checkout') {
      parallel {
        stage('Checkout') {
          steps {
            sh '''pwd
ls'''
          }
        }
        stage('Directory') {
          steps {
            sh '''cd Java
ls'''
          }
        }
      }
    }
    stage('Done') {
      steps {
        echo 'Done'
      }
    }
  }
}