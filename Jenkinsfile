pipeline {
    agent any
   
    stages {
        stage('Build') { 
            steps {
                def mvn_version = ''
                withEnv( ["PATH+MAVEN=${tool mvn_version}/bin"] ) 
                        {   
      sh  'mvn clean package'
                    }
                
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
            post {
                always {
                    junit 'target/surefire-reports/*.xml'
                }
            }
        }
        stage('Deliver') {
            steps {
                sh './jenkins/scripts/deliver.sh'
            }
        }
    }
}
