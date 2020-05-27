pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build 1') {
          steps {
            echo 'Build in Progress'
          }
        }

        stage('Build2') {
          steps {
            echo 'Build in parallel'
          }
        }

      }
    }

    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            echo 'Deploy in Progress 1'
          }
        }

        stage('Deploy2') {
          steps {
            echo 'Deploy in paralllel'
          }
        }

      }
    }

    stage('Test') {
      parallel {
        stage('Test1') {
          steps {
            echo 'Test in progress 1'
          }
        }

        stage('Test2') {
          steps {
            echo 'Test in parallel'
          }
        }

      }
    }

  }
}