pipeline {
  agent any 
  stages {
    stage ('Build') {
      steps {
        echo 'Build automation is running'
        sh './gradlew build --no daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
