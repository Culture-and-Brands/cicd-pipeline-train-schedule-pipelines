pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo "running the building stage automation...."
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
