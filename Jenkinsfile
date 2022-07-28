pipeline {
	agent { 
		docker { image 'maven:3.8.6-jdk-11-slim' } 
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


