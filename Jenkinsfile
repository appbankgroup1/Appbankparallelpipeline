pipeline{
	agent any 
	stages{
		stage('1-clone'){
			steps{
				echo "we are Appbank Group 1 Engineers"
			}
		}
		stage('2-Parallelpipeline'){
			parallel{
				stage('1-parallelsubjob1'){
					steps{
						sh 'bash -x /var/lib/jenkins/checkops.sh'                                                                                                                       
					}
			    }
			    stage('2-parallelsubjob2'){
			    	steps{
			    		sh 'bash -x /var/lib/jenkins/jenstatus.sh'
			    	}
			    }
			}	
		}
	}
}