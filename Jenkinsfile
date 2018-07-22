pipeline {
	agent any;
	stages {
		stage('Buil the project using Gradle') {
			steps {
				sh './gradlew build --no-daemon'
				sh 'pwd && ls -larth'
				archiveArtifacts artifacts : '/dist/trainSchedule.zip'
			}
		}
	}
}
