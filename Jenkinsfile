Pipeline{
    agent any
  stages{
        stage('clean workspace')
    {
      steps{
        sh ' rm -r *'
        sh ' rm -r ../../../../www/html/*'
          }
      }
    
    stage('git scm clone'){
      
      steps{
        
          sh ' git clone https://github.com/pavan731/constructive.git -b master '
        
          }
    }
    stage('deploy'){
      steps{
        sh ' mv constructive/* ../../../../www/html'
          }
    }
    
  }
}
      
