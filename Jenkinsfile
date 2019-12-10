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
          steps {
            sh 'maven'
           }

        }
    }
}
