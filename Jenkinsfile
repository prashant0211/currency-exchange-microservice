pipeline {
	agent { 
		docker { image 'python:3.10.5-alpine3.16' } 
		}
	stages {
		stage('build') {
			steps{
				echo "this is build"
				sh "mvn --version"
			}
		}
		stage('test') {
			steps {
				echo "this is test"
			}
		}

	}
	post {
		always {
			echo "always print this"
		}
		success {
			echo "this is success  "
		}
		failure {
			echo "this is failure"
		}
	}
}


