pipeline {
    agent any 
    
stage('Build and publish') {

  steps {
    sh "mvn -B -s settings.xml deploy"
  }
        }
        stage('Test') { 
            steps {
                sh 'echo testing step'
            }
        }
    }
}
