pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo'Running build automation'
        sh './gradlew buid --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
