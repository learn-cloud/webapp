pipeline{
	agent any
	stages{
		stage('Clean'){
			deleteDir()
			steps{
					echo "Deleting WorkSpace"
					sh 'ls -ltr'
			}
		}

		stage('Checkout'){
			checkout scm
		}

		stage('Compile'){
			steps{
				sh 'mvn complile'
			}
		}
	}
}
