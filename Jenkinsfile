pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello World'
      }
    }
    stage('Testing') {
      steps {
        sh 'sleep 5'
        sh 'echo Tests Completed!'
      }
    }
    stage('Publish Event') {
      steps {
        script {
          publishEvent simpleEvent('testingCompleted')
        }

      }
    }
  }
}