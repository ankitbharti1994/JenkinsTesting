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
        sh 'xcodebuild test -workspace JenkingsTesting/JenkingsTesting.xcworkspace -scheme "JenkingsTestingTests" -destination \'platform=iOS Simulator,name=iPhone 8\''
      }
    }
  }
}
