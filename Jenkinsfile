pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
          sh 'xcodebuild -workspace JenkingsTesting/JenkingsTesting.xcworkspace -scheme "JenkingsTesting" -destination \'platform=iOS Simulator,name=iPhone 8\''
      }
    }
    stage('Test') {
      steps {
        echo 'Testing...'
      }
    }
  }
}
