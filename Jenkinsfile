pipeline {

   agent any
   stages {

      stage ('build') {
         
         steps {
            echo "Runninig Build automation"
            sh ./gradlew build --no-daemon   
         }
      }
   }
   post {
      success {
         archiveArtifacts artifacts: 'dist/trainSchedule.zip',
      }
   }
}
