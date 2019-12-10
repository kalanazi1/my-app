pipeline {
    agent any
    tools { 
        maven 'Maven' 
        jdk 'JDK' 
    }
stage('Build and publish') {
  steps {
    sh "mvn -B -s settings.xml deploy"
  }
}

