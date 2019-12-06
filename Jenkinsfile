pipeline {
    agent any
      tools {
        maven 'Maven 3.6.3'
        jdk 'JDK'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'echo first step'
            }
        }
        stage('Test') { 
            steps {
                sh 'echo testing step'
            }
        }
    }
}
