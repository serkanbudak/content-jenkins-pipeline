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

      post {
        always {
          deleteDir()
        }
      }
    }
  }
}
