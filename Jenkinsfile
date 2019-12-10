pipeline {
    agent any
    tools { 
        maven 'Maven' 
    }
stage('Build and publish') {
  steps {
    sh "mvn -B -s POM.xml deploy"
  }
}

