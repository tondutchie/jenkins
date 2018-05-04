pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }
         stage ('Build') {
            steps {
                echo 'Build'
                sh "/usr/bin/xcodebuild build -workspace ./Users/tondutchie/Documents/tdcDocuments/TDC/Coding/FizzBuzzGit/FizzBuzzTest/FizzBuzz.xcworkspace -scheme FizzBuzz -destination 'platform=iOS Simulator,name=iPhone X,OS=11.2'"
            }
        }
    }
   }