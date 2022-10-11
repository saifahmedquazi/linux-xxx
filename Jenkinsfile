pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date
'''
        sleep 5
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test stage'
          }
        }

        stage('quality') {
          steps {
            echo 'quality cheak'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy successfull'
      }
    }

  }
}