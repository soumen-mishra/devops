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
    
    stage('Run Script') {
      steps {
        echo 'Executing Shell Script!'
        chmod +x 'job.sh'
        sh('job.sh')
      }
    }
  }
}
