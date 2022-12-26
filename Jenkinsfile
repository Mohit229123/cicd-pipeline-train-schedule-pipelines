jenkins {
    agent any
    stages {
        stage ('Build') {
            echo 'Running build automation'
            sh './gradlew build --no-daemon'
            archiveArtifcats artifacts: 'dist/trainSchedule.zip'
        }
    }
}