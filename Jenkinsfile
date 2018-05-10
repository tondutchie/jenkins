pipeline {

  def GIT_URL = 'https://github.com/tondutchie/jenkins'
  agent any
  stages {

  stage('prepare') {

      steps {
        git url: "${GIT_URL}"
        sh "git clean -fdx"
      }
    }


    stage('test') {

      steps {
        sh 'fastlane tests'
      }
    }

    stage('beta') {

      steps {
        sh 'fastlane make_ipa'
      }
    }
    }
   }