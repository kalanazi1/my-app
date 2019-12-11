pipeline {
    agent any
    
    stages {
        stage('Initialize') {
            steps {
                echo "PATH = ${PATH}"
                echo "M2_HOME = ${M2_HOME}"
            }
           
        }
        stage ('SCM Checkout'){ 
   				steps{
   					git 'https://github.com/kalanazi1/my-app'
   					}
					mvnHome = tool 'M3'
  						}
        stage('Build') { 
            steps { 
                    sh  'mvn clean package'
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
