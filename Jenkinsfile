pipeline {
  agents any
    stages {
      stage ('build') {
        steps {
          echo "running build automation"
          sh './gradle build --no-daemon'
          archiveArtifacts artifacts: 'dist/trainSchedule.zip'
        }
      }
    }
}
