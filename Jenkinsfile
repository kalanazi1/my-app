pipeline {
    agent any
      tools {
        maven 'Maven'
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
