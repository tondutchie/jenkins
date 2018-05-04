pipeline {
  agent any

  stages {
    stage('Test') {
      steps {
        sh 'fastlane tests'
      }
     }

     stage('BuildIpa') {
     steps {
        sh 'fastlane make_ipa'
      }
     }

    }
   }