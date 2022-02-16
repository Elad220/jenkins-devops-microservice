pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
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
