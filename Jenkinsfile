pipeline {
    agent any
      tools {
        maven 'Maven'
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
