pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }
           
        stage ('Unit Test') {
            steps {
                echo 'Unit Test'
                sh "/usr/bin/xcodebuild test -workspace ./FizzBuzz.xcworkspace -scheme FizzBuzz -destination 'platform=iOS Simulator,name=iPhone X,OS=11.2'"
            }
        }

    }
   }
 }