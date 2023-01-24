pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''ls
mkdir Jenkins'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test pass'
          }
        }

        stage('Integration') {
          steps {
            sh '''ls
mkdir integration test'''
          }
        }

      }
    }

  }
}