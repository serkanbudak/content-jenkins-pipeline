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
        }
      }
      
            stages {
        stage('Checout') {
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
