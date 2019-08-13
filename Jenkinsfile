pipeline {
  agent any
  stages {
    stage('initialize') {
      steps {
        echo 'This is minimal pipeline'
      }
    }
    stage('Compile') {
      steps {
        bat 'compile'
      }
    }
  }
}