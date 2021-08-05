node {
  stages { 
    stage ('Build') {
      step {
        sh './gradlew build --no-daemon'
      }
    }
  }
  post {
      archiveArtifacts artifacts: '*', fingerprint: true
    }
  }
}
