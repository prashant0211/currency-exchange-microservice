pipeline {
    agent {
        docker { image 'node:16.13.1-alpine' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
/*
pipeline {
	agent { 
		docker { 
			image 'maven:latest'
			args '-v /var/run/docker.sock:/var/run/docker.sock' 
		} 
	}
	stages {
		stage('build') {
			steps{
        		sh 'docker run maven:3.8.6-jdk-11-slim'
				
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

*/