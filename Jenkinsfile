pipeline {
  agent any
  
  stages {
    stage('One') {
      when { expression {  env.GIT_PREVIOUS_COMMIT == env.GIT_COMMIT } }
      steps {
        sh '''
          echo Hello
          env
        '''
      }
    }
    
  }
  
}
