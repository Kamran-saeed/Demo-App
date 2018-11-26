pipeline{
   agent any
   tools {
        maven 'Apache Maven 3.6.0'
        jdk 'JDK 9'
   }
   stages {
      stage('Pull') { 
         steps{
           git 'https://github.com/talhakhannnnn/Demo-App.git'
         }
       }
      stage ('Build'){
         steps{
               bat "mvn clean install"
         }
      } 
      stage ('Test'){
         steps{
               bat "mvn test"
         }
      }
      
   }
}
