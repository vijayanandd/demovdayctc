pipeline {
	agent any
	
	stages {
		stage ('compile') {
			steps {
				sh 'mvn clean compile'
			}
		}
		
		stage ('Testing') {
			steps {
					sh 'mvn test'
			}
		}
		
		stage ('package') {
			steps {
					sh 'mvn package'
			}
		}		
				
	}
}