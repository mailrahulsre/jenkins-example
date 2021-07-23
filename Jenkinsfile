pipeline {
    agent any
    
       
    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "maven-3.6.3"
    }

    stages {
        stage ('Compile Stage') {

            steps {
           
                    sh 'mvn clean compile'
            
            }
        }

        stage ('Testing Stage') {

            steps {
              
                    sh 'mvn test'
          
            }
        }


        stage ('Deployment Stage') {
            steps {
             
                    sh 'mvn deploy'
             
            }
        }
    }
}
