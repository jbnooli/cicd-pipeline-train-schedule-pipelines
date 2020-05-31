pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        echo 'In build stage'
        sh './gradlew build --no --daemon'
        archiveArtifacts arctifacts:'dist/trainSchedule.zip'
        echo 'Steps completed'
      }
    }
  }

}
