pipeline {
  agent none

  stages {
    stage('Hello World') {
      agent any

      stages {
        stage('Nested') {
          steps {
            echo 'Hi!'
          }
           stage('Checkout') {
          steps {
            checkout scm
          }
        }
      }
      
           
      post {
        always {
          deleteDir()
        }
      }
    }
  }
}
