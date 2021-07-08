pipeline
 {
  agent any

  tools
   {
    maven 'MAVEN_HOME'
    jdk 'JAVA_HOME'
   }


    stages {
        stage ('Build Stage') {

            steps {
               
                    bat 'mvn clean compile'
             
            }
        }

        stage ('Testing Stage') {

            steps {
              
                    bat 'mvn test'
              
            }
        }


    }

 }
