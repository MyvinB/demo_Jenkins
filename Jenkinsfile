pipeline {
  agent {
    docker {
      image 'maven:3.5-jdk-8-slim'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'mvn clean'
      }
    }
    stage('install') {
      steps {
        sh 'mvn install package'
      }
    }
  }
}