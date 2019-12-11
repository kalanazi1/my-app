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
                sh 'mvn -Dmaven.test.failure.ignore=true install' 
            }
            post {
                success {
                    junit 'target/surefire-reports/**/*.xml' 
                }
            }
        }
    }
}
