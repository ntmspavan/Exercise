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
            sh '''BNAME="echo ${BRANCH_NAME}|awk -F \'/\' \'{print $2}\'"
echo "${BNAME}"'''
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