pipeline {
	agent none

	options {
		buildDiscarder(logRotator(numToKeepStr: '5'))
		disableConcurrentBuilds()
	}

	stages {
		stage('Build') {
			agent {
				docker {
					image 'registry.jeroensteenbeeke.nl/jekyll-builder:latest'
					label 'docker'
				}
			}

			steps {
				sh 'jekyll build'
			}
		}
	}
}
