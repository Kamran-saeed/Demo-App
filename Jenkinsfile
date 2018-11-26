pipeline{
   agent any
   tools {
        maven 'mvn-3.6.0'
        jdk 'myJDK'
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
