pipeline {
  agent any 
  stages {
    stage('Build') {
      steps {
        ehco 'Running build automation'
        sh './gradlew build --no-daemon'
        archieveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
