pipeline {
	agent {docker {image 'maven:3.6.3'} args '-u root:root'}
	stages {
		stage('Build') {
			steps {
				sh 'mvn --version'
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
