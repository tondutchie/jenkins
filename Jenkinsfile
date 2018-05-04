pipeline {
  agent any

  stages {
    stage('Build ipa') {
      when {
        expression {
          return params.type == "test"
        }
      }
      steps {
        sh 'fastlane make_ipa'
      }
     }
    }
   }