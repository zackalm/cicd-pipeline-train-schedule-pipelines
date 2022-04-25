pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running Build Automation'
        sh './gradlew Build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
