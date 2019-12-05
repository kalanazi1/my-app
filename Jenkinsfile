pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh 'mvn package'
            }
        }
        stage('Test') { 
            steps {
                sh 'echo testing step'
            }
        }
    }
}
