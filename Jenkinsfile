pipeline{

	agent any
	tools{
		maven 'Maven Maven 3.8.6'
	}
	stages{
	
	   stage('build'){
		steps{
		  sh 'mvn compile'
		}
	   }
	
	   stage('test'){
		steps{
		  sh 'mvn clean test'
		}
	   }
	
	   stage('package'){
		steps{
		  sh 'package -DskipTests'
		}
	   }
	}
}