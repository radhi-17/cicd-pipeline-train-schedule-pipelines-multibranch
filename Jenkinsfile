pipeline {
  agent any
  stages {
    stage ('Git') {
     steps {
       echo 'clone the repo'
       echo 'gradle view'
     }
   }
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
     steps {
        echo 'This is pipeline sccript'
     }
    }
  }
}
