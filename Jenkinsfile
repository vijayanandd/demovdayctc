pipeline {
	agent any
	
	stages {
		stage ('compile') {
			steps {
				withMaven(maven : 'apache-maven-3.5.4') {
					bat 'mvn clean compile'
				}
			}
		}
		
		stage ('Testing') {
			steps {
				withMaven(maven : 'apache-maven-3.5.4') {
					bat 'mvn test'
				}
			}
		}
		
		stage ('package') {
			steps {
				withMaven(maven : 'apache-maven-3.5.4') {
					bat 'mvn package'
				}
			}
		}		
				
	}
}