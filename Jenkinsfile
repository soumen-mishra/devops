pipeline {
  agent any
  
  options {
    skipDefaultCheckout(true)
  }
  
  stages {
    stage('Git Checkout') {
        steps {
          echo 'Git Repository Checkout !'
          git 'https://github.com/soumen-mishra/devops.git'
        }
    }
    
    stage('Demo Stage') {
      steps {
        echo 'Hello world!'
      }
    }
  }
}
