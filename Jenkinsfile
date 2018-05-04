pipeline {
  agent any
  stages {
    stage('test') {
      when {
        expression {
          return params.type == "test"
        }
      }
      steps {
        sh 'fastlane tests'
      }
    }

    stage('beta') {
      when {
        branch "release/*"
        expression {
          return params.type != "release"
        }
      }
      steps {
        sh 'fastlane make_ipa'
      }
    }
    }
   }