pipeline {
    agent any 
    
    environment{
        PATH = "/opt/maven/bin:$PATH"
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
