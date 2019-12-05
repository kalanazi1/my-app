pipeline {
    agent any 
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
