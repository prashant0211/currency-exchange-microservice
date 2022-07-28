pipeline {
	agent { docker {image 'maven:3.6.3' } }
	stages {
		stage('build') {
			steps{
				echo "this is build"
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


