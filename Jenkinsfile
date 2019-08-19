pipeline {
  agent {
    docker {
      image 'maven:3.3.9-jdk-8'
    }

  }
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