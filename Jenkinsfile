pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'build the code'
          }
        }

        stage('TestBuild') {
          steps {
            echo 'Test Build'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy to app server'
      }
    }

  }
}