node{
  
   stage('git clone'){
     git credentialsId: 'b9900d3a-ead8-44d4-bce8-ef278b9eb584', url: 'https://github.com/myproject-ec-apps/java-web-app-docker.git'
  }

   stage('build the code'){
     def mavenHome= tool name: "maven",type: "maven"
     sh "${mavenHome}/bin/mvn clean package"
     
   }

}

  