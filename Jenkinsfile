pipeline {
	agent any
	
	stages {
		stage ('compile') {
			steps {
				withMaven(maven : 'apache-maven-3.5.4') {
					powershell 'mvn clean compile'
				}
			}
		}
		
		stage ('Testing') {
			steps {
				withMaven(maven : 'apache-maven-3.5.4') {
					powershell 'mvn test'
				}
			}
		}
		
		stage ('package') {
			steps {
				withMaven(maven : 'apache-maven-3.5.4') {
					powershell 'mvn package'
				}
			}
		}		
				
	}
}