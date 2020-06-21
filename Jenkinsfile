pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'build the code'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy to app server'
      }
    }

    stage('crone') {
      steps {
        build(job: 'jenkinspipeline', quietPeriod: 10, wait: true)
      }
    }

  }
}