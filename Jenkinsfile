pipeline {
  agent any
  
  stages {
    
    stage('Different Commits') {
      when { expression {  GIT_PREVIOUS_COMMIT != GIT_COMMIT } }
      steps {
        sh '''
          echo "Run this only if commits are different"
        '''
      }
    }
    
    stage('Same Commits') {
      when { expression {  GIT_PREVIOUS_COMMIT = GIT_COMMIT } }
      steps {
        sh '''
          echo "Run this only if commits are same"
        '''
      }
    }
    
  }
  
}
