#!groovy

pipeline{
		agent any
		stages{
			stage('clean the workspace'){
					steps{
							echo 'deleting the workspace'
							deleteDir()
					}
			}
			stage('checkout the code'){
					steps{
			 				echo "Download the code from github"
							checkout scm					
					}

			}
			stage('compile the code'){
					steps{
						script{
								echo 'compile the code'
								sh 'mvn compile'
						}
					}
					
			}			
			stage('packgae the code'){
					steps{
							script{
									echo 'packaging the code'
									sh 'mvn package'
							}
					}	
			}
		}
}
