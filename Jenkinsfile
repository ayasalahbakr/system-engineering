pipeline {
    agent any
    stages {
		stage ('Java Build') {
			steps {
		                sh """
				
				  			"""
				  
			    	}
				}
		stage('Docker') {
        	steps {
     					sh """
                      
				                docker-compose build -t ayasalah/devops-assessment:V0.1 .            
				                docker-compose push -p ayasalah -u V0daf0ne_6392 ayasalah/devops-assessment:V0.1                             
			     			"""

			}
        }
        
        stage('Deploy Docker') {
	     	steps {
            sh """
                docker-compose up
                """
	       	}
   	 	}
    }
}