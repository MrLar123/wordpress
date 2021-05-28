pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('error') {
          steps {
            echo 'hello'
          }
        }

        stage('deploy') {
          steps {
            timestamps() {
              sh '''ls -l
pwd'''
            }

          }
        }

      }
    }

  }
}