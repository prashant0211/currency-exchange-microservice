/*node {
	stage('Build') {
		echo "Build prashant"
	}
	stage('Test') {
		echo "Test"
	}
}*/
pipeline{
	agent any
	stages{
		stage("build"){
			steps{
				echo "this is build"
			}
		}
		stage("test"){
			steps{
				echo "this is test"
			}
		}
	}post{
		always{
			echo "always print this"
		}
		success{
			echo "this is success  "
		}
		failure{
			echo "this is failure"
		}
	}
}
