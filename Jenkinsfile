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
            sh '''echo "----This is for changing Directory---" 
cd Java
ls'''
            sh '''echo "${BRANCH_NAME}|awk -F \'/\' \'{print $2}\'"
'''
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