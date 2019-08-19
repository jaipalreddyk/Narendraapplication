pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        bat 'compile'
      }
    }
    stage('Build') {
      steps {
        build 'build'
      }
    }
    stage('sonarcube') {
      steps {
        withSonarQubeEnv 'sonar'
      }
    }
    stage('test') {
      steps {
        junit 'junit'
      }
    }
    stage('deploy') {
      steps {
        archiveArtifacts 'artifa'
      }
    }
    stage('release') {
      steps {
        echo 'print'
      }
    }
  }
}