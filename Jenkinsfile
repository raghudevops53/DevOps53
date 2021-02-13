pipeline {
  agent any
  
  stages {
    stage('One') {
      when { expression {  GIT_PREVIOUS_COMMIT != GIT_COMMIT } }
      steps {
        sh '''
          echo Hello
          env
        '''
      }
    }
    
  }
  
}
