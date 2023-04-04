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
				stage('1-parallelsubkofo'){
					steps{
						sh 'bash -x /var/lib/jenkins/checkops.sh'                                                                                                                       
					}
			    }
			    stage('2-parallelsubtee'){
			    	steps{
			    		sh 'bash -x /var/lib/jenkins/jenstatus.sh'
			    	}
			    }  
			}	
		}
        stage('3-Parallelpipeline'){
            parallel{
                stage('1-parallelsubmark'){
                    steps{
                        sh 'bash -x /var/lib/jenkins/workspace/Appbankparallelpipeline/mark.sh'
                    }
                }
                stage('2-parallelsubevert'){
                    steps{
                        sh 'bash -x /var/lib/jenkins/workspace/Appbankparallelpipeline/evert.sh'
                    }
                }
            }
        }
        stage('4-Parallelpipeline'){
			parallel{
				stage('1-parallelsubLacaine'){
					steps{
						sh 'bash -x /var/lib/jenkins/checkops.sh'                                                                                                                       
					}
			    }
			    stage('2-parallelsubYovwi'){
			    	steps{
			    		sh 'bash -x /var/lib/jenkins/jenstatus.sh'
			    	}
			    }  
			}	
		}
        stage('5-Parallelpipeline'){
            parallel{
                stage('1-parallelsubsam'){
                    steps{
                        sh 'bash -x /var/lib/jenkins/workspace/Appbankparallelpipeline/mark.sh'
                    }
                }
                stage('2-parallelsubkafayat'){
                    steps{
                        sh 'bash -x /var/lib/jenkins/workspace/Appbankparallelpipeline/evert.sh'
                    }
                }
            }
        }
	}
}