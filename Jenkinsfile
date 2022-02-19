pipeline {
	agent any
	environment {
		dockerHome = tool 'docker'
		mavenHome = tool 'maven'
		PATH = '$dockerHome/bin:$mavenHome/bin:$PATH'
	}
	stages {
		stage('Build') {
			steps {
				sh 'mvn --version'
				// sh 'docker version'
				echo 'build'
			}
		}
		stage('Test') {
			steps {
				echo 'Test'
			}
		}
		stage('Integration test') {
			steps {
				echo 'Integration test'
			}
		}
	}
	
	post {
		always {
			echo 'Post always'
		}
		success {
			echo 'Post success'
		}
		failure {
			echo 'Post failure'
		}
	}
}
