pipeline{
	agent any
	stages{
		stage('Clean'){
			deleteDir()
			script{
					echo "Deleting WorkSpace"
					sh 'ls -ltr'
			}
		}

		stage('Checkout'){
			checkout scm
		}

		stage('Compile'){
			script{
				sh 'mvn complile'
			}
		}
	}
}
