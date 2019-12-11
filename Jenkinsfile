pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'java'
    }
    stages {
        stage('Initialize') {
            steps {
		    //def mvn_version = 'M3'
//withEnv( ["PATH+MAVEN=${tool mvn_version}/bin"] ) {
  //sh "mvn clean package"
//}
		sh '''    
                echo "PATH = ${PATH}"
                echo "M2_HOME = ${M2_HOME}"
		'''
            }
        }

        stage ('Build') {
            steps {
                sh 'mvn package' 
	    	}
            }
	    stage('Test') {
		    steps {
			    sh 'mvn test'
	    }
            post {
                success {
                    junit 'target/surefire-reports/**/*.xml' 
                }
            }
        }
    }
}
