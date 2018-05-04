pipeline {
  agent any

  stages {
    stage('Test') {
      when {
        expression {
          return params.type == "test"
        }
      }
      steps {
        sh 'fastlane tests'
      }
     }
    }
   }