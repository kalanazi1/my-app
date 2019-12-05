pipeline {
    agent any 
     tools {
        maven 'Maven 3.6.3'
        jdk 'jdk'
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
