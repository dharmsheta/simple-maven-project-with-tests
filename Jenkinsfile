pipeline {
  agent any
  stages {
    stage('Preparation') {
      steps {
        parallel(
          "Preparation": {
            echo 'Preparation phase only'
            sh 'echo "hello world"'
            
          },
          "build": {
            sh 'echo "hello world"'
            
          }
        )
      }
    }
    stage('Qualify') {
      steps {
        sh 'echo "Qualification"'
      }
    }
    stage('Final State') {
      steps {
        sh 'echo "finally done"'
      }
    }
  }
}