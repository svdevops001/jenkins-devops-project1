pipeline {
	// agent any
	agent { docker { image 'nginx:latest'} }
	stages {
		stage('Build') {
			steps {
				sh "nginx --version"
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
