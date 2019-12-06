pipeline {
    agent any 
    tool {
          jdk "Java-1.8"
          maven "Maven-3.6.3"
    }
    
    stage {
        stage('Clone sources'){
            steps {
                git url: 'https://github.com/kalanazi1/my-app'
            
            }
        }
