pipeline {
    agent any 
    
    environment{
        PATH = "/var/lib/jenkins/tools/hudson.tasks.Maven_MavenInstallation/M3"
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
