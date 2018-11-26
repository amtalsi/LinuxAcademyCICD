pipeline {
	agent any;
	stages {
		stage('building') {
			steps {
				sh './gradlew build --no-daemon'
				sh 'pwd && ls -larth'
				archiveArtifacts artifacts : '/dist/trainSchedule.zip'
			}
		}
	}
}
