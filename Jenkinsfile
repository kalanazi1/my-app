pipeline {
    agent any 
     tools {
        maven 'mvn'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'echo mvn package'
            }
        }
        stage('Test') { 
            steps {
                sh 'echo testing step'
            }
        }
    }
}
