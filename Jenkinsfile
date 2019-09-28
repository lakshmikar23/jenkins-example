pipeline {
	agent any
	stages {
		stage('---clean---'){
			steps {
				tool name: 'maven_3.6.1', type: 'maven'
				sh "mvn clean"
			}
		}
		stage('---test---') {
			steps {
				tool name: 'Maven-3.5.4', type: 'maven'
				sh "mvn test"
			}
		}
		stage('---package---'){
			steps {
				tool name: 'Maven-3.3.3', type: 'maven'
				sh "mvn package"
			}
		}
	}
}
