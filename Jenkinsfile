pipeline {
  agent any
  stages {
    stage ('start') {
      steps {
        echo 'starting the build'
        }
        }
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
