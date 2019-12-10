node {
  stage ('SCM Checkout'){ 
   git 'https://github.com/kalanazi1/my-app'
  }
  stage ('Compile-Package'){
    def mvnHome= tool name: 'Maven', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
}
