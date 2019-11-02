pipeline {
  agent {
    docker {
      image 'maven:3.5-jdk-8-slim'
    }

  }
  stages {
    stage('build') {
      steps {
        sh '''echo "hello wolrd"
mvn clean'''
      }
    }
    stage('panda') {
      steps {
        sh 'mvn install package'
      }
    }
  }
}