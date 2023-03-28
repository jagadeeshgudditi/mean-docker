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
             /*sh 'docker-compose up' */
  /*       }*/ 
     /*}*/
     stage('Docker Build') {
        	agent any
       steps {
      	  sh 'docker-compose up'
      }
    }
    
    stage('Testing'){
         steps {
             echo 'Testing..'
             }
    }
    }
}
