pipeline{
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
                  
		  sh ' git clone https://gitlab.com/spshariq6/wedding.git -b master '

	     }
 
	}
	stage('deploy'){
              steps{
                sh 'mv wedding/* ../../../../www/html'
	      }
	}
     
   }
  
}

