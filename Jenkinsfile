
//Declarative
pipeline {
	//agent any
	agent { docker { image 'maven:3.8.4' args '-e HOME=/tmp/home'} }
	stages {
		stage('Build') {
			steps {
				sh 'mvn --version'
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
