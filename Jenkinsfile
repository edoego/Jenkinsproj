node{
   stage('SCM Checkout'){
     git 'https://github.com/edoego/spring-petclinic.git'
   }
   stage('Compile-Package'){
      // Get maven home path
      def mvnHome =  tool name: 'maven-3', type: 'maven'   
      sh "${mvnHome}/bin/mvn package"
   }

}
