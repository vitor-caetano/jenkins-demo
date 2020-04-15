pipeline {
  agent any
  options {
    buildDiscarder logRotator(numToKeepStr: '5')
    disableConcurrentBuilds()
  }
  stages {
    stage("Run demo-shared-libraries") {
      steps {
          echoWorkspace()
      }
    }
  }
  post {
      always {
          echo "Bye!"
      }
    }
}