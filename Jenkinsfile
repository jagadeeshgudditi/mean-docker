pipeline {
 agent any
     stages {
         stage('Clone Repository') {
         /* Cloning the repository to our workspace */
         steps {
         checkout scm
         }
    }
    
     stage('Build Image') {
         steps {
         sh ' docker build .'
         }
    } 
      
    stage('Run Image') {
         
         steps {
         sh ' docker run -d -p 8050:8000 --name meanapp mean-docker_angular'
         }
    }
    stage('Testing'){
         steps {
             echo 'Testing..'
             }
    }
    }
}
