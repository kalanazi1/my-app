pipeline {
  agent any
  stages {
    stage("Build") {
      steps {
        sh 'mvn -v'
      }
    }
    stage("Testing") {
      parallel {
        stage("Unit Tests") {
          agent { docker 'openjdk:7-jdk-alpine' }
          steps {
            sh 'java -version'
           }

        }
    }
}
