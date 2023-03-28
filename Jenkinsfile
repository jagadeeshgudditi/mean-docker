pipeline {
 agent any
     stages {
         stage('Clone Repository') {
         /* Cloning the repository to our workspace */
         steps {
         checkout scm
         }
    }
    
     /*stage('Build Image and Run Image') { */
        /* steps { */
          /*sh 'cd mean-docker'*/
             */sh 'docker-compose -f 'docker-compose.debug.yml' up' */
  /*       }*/ 
     */}*/
     stage('Docker Build') {
        	agent any
       steps {
      	  sh 'docker build -t meanapp:latest .'
      }
    }
    
    stage('Testing'){
         steps {
             echo 'Testing..'
             }
    }
    }
}
