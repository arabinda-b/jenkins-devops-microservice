
//Declarative
pipeline {
	//agent any
	agent { docker 'maven:3.8.1-adoptopenjdk-11' }
	stages {
		stage('Build') {
			steps {
				echo "Build"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	}
	post {
		always {
			echo 'I am awesome. I run always.'
		}
		success {
			echo 'I run when you succeed..'
		}
		failure {
			echo 'I run when you fail.'
		}
	}
}
