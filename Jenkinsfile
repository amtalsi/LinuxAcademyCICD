pipeline {
	agent any;
	stages {
		stage('Buil the project using Gradle') {
			steps {
				sh './gradlew build --no-daemon'
			}
		}
	}
}
