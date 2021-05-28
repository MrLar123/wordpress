pipeline {
  agent any
  stages {
    stage('alpha') {
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

    stage('beta') {
      parallel {
        stage('beta') {
          steps {
            sh 'echo start beta'
            echo 'TO Beta'
          }
        }

        stage('deploy') {
          steps {
            echo 'success!'
          }
        }

      }
    }

  }
}