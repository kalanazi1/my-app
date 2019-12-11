pipeline {
	agent {master} 
    stages{
  stage ('SCM Checkout'){ 
   steps{
   git 'https://github.com/kalanazi1/my-app'
   }
  }
  stage ('Compile-Package'){
    steps{
	
    sh 'mvn package'
	}
  }
}
}
