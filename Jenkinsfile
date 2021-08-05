Fork this project in GitHub: https://github.com/linuxacademy/cicd-pipeline-train-schedule-pipelines

On the master branch, create a Jenkinsfile. In the Jenkinsfile, create a stage that executes the gradle
build with ./gradlew build --no-daemon and archives the dist/trainSchedule.zip artifact.

Configure the train-schedule multibranch pipeline project in Jenkins to build 
the source code from your GitHub fork and execute the build on the master branch successfully.
This should produce the dist/trainSchedule.zip archived artifact.
node {
  agent { any }
  stage ('Build') {
    step {
      sh './gradlew build --no-daemon'
    }
    step {
      archiveArtifacts artifacts: '*'
    }
  }
}

