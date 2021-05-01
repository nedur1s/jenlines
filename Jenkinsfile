pipeline {
     agent any
     tools {
         jdk 'jdk1.8'
       maven 'maven3'
     }
  stage{
    stage('pull code from git'){
         steps{ 
           echo 'pulling code from git repo'
           git https://github.com/nedur1s/jenlines.git
         }
    }
    stage('maven clean & buld'){
      steps{
        echo 'mavan cleaned and buld'
        sh 'mvn clean'
        sh ' mvn install'
      }
    }
  }
}
  
