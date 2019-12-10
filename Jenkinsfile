pipeline {
 Stages{
  Stage ('SCM Checkout'){ 
   steps{
   git 'https://github.com/kalanazi1/my-app'
   }
  }
  Stage ('Compile-Package'){
    steps{
	  def mvnHome= tool name: 'Maven', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
	}
  }
}
}
