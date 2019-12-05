pipeline {
    agent any 
    stages {
        stage('Preparation') {
            steps {
                      sh 'mvn package'
            }
        }
    stages {
        stage('Build') { 
            steps {
                sh 'echo mvn package'
            }
        }
    }
}
