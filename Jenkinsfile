pipeline {
	agent {
		docker {
			image 'node:13.8'
		}
	}
	stages {
		stage('Build') {
			steps {
				sh 'node --version'
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
