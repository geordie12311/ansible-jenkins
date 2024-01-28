pipeline{
	agent any
	stages{
  		stage('Setup'){
      			steps{
				sh 'chmod +x install.sh'
        			sh './install.sh'
      			}
    		}
    		stage('Test'){
      			steps{
				 sh '''#!/bin/bash
				     source env/bin/activate	
                		     python -m unittest
				     '''
               			}
   		}
	}
}
