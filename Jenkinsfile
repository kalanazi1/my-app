pipeline {
    agent any
      tools {
        maven 'Maven'
    }
    stages {
 
        stage ('Build') {
            steps {
                sh 'mvn -Dmaven.test.failure.ignore=true install' 
        
                }
            }
        }
    }
}
