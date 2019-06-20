#!groovy

pipeline
{
     agent any
     stages
     {
        stage('clean')
        {
            steps
             {
                 deleteDir()
                 echo "Cleaning completed"
             }

        }

        stage('Checkout')
        {
            checkout scm
        }
     }
}
