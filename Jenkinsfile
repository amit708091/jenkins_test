pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
ls
date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
          }
        }

        stage('test_part') {
          steps {
            echo 'test_part'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        sleep 10
      }
    }

    stage('proud') {
      steps {
        echo 'success'
      }
    }

  }
}