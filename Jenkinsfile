pipeline {
    agent any 
    stages {
    stage("Build") {
            environment {
                MVN_COMMAND = "mvn clean package"
                TEST_REPORTS = "target/surefire-reports/*.xml"
            }
        stage('Test') { 
            steps {
                sh 'echo testing step'
            }
        }
    }
}
