pipeline {
	// agent any
	agent { docker { image 'maven:3.8.5-openjdk-8-slim'} }
	stages {
		stage('Build') {
			steps {
				// sh "mvn --version"
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
			echo "I'm awsome, I run always"
		}
		success {
			echo "I run when you are successful"
		}
		failure {
			echo "I run when you fail"
		}
	}
	
	}
