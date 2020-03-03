pipeline {
    stages {
		stage ('Java Build') {
			steps {
		                sh """
				
				  			"""
				  
			    	}
				}
		stage('Docker') {
        	steps {
     	withCredentials([usernamePassword(credentialsId: 'dockerhub', usernameVariable: 'ayasalah', passwordVariable: 'V0daf0ne_6392')]) {
          					sh """
				                docker-compose build -t ayasalah/devops-assessment:V0.1 .            
				                docker-compose push ayasalah/devops-assessment:V0.1                             
			     			"""

			}
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