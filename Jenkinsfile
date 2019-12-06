pipeline {
    agent any 
    
    environment{
        PATH = "/var/lib/jenkins/"
    }
    stages {
        stage('Build') { 
            steps {
                sh "mvn clean package"
            }
        }
        stage('Test') { 
            steps {
                sh 'echo testing step'
            }
        }
    }
}
