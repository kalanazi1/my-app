pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh 'mvn clean install test'
            }
        }
        stage('Test') { 
            steps {
                sh 'echo testing step'
            }
        }
    }
}
