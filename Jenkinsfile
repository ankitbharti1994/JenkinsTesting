pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
          sh 'xcodebuild -workspace JenkinsTesting.xcworkspace -scheme "JenkinsTesting" -destination \'platform=iOS Simulator,name=iPhone 8\''
      }
    }
    stage('Test') {
      steps {
        echo 'Testing...'
      }
    }
  }
}
