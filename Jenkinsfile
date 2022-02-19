pipeline {
	agent any
	environment {
		maven_home = tool 'maven'
		docker_home = tool 'docker'
		PATH = '$docker_home/bin:$maven_home/bin:$PATH'
	}
	stages {
		stage('Build') {
			steps {
				sh 'maven --version'
				sh 'docker version'
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
