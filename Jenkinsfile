pipeline {
  agent any
  
  stages {
    stage('Build Docker Image') {
      steps {
        sh 'docker build -t devsecfrat:$BUILD_NUMBER .'
        }
       }
    
    stage('Test Run') {
          steps {
            sh 'docker run -d devsecfrat:$BUILD_NUMBER'
          }
          }
      }
     }
      
