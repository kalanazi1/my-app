pipeline {
 agent any
    options {
        skipStagesAfterUnstable()
    }
 stages{
  stage ('SCM Checkout'){ 
   steps{
   git 'https://github.com/kalanazi1/my-app'
   }
  }
  stage ('Compile-Package'){
    steps{
	  def mvnHome= "tool name: 'Maven', type: 'maven'"
    sh "${mvnHome}/bin/mvn package"
	}
  }
}
}
