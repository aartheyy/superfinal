pipeline {
    agent any
  
    stages {
        stage ('Compile Stage') {
            steps {
                cd Java_WebApp-master/Java_WebApp-master/java-webapp
                sh 'mvn clean compile'
            }    
         }
                          
         stage ('Testing Stage') {
           steps {
               cd Java_WebApp-master/Java_WebApp-master/java-webapp
               sh 'mvn test'
            }
         } 
       
       stage ('Deployment Stage') {
         steps {
             cd Java_WebApp-master/Java_WebApp-master/java-webapp
             sh 'mvn package'
         }
       }
    }    
}
