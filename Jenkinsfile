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
            sh '''branch = "echo ${BRANCH_NAME}"
echo "${branch}"'''
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