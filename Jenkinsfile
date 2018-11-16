pipeline {
	agent {
		docker {
			image 'registry.jeroensteenbeeke.nl/jekyll-builder:latest'
			label 'docker'
		}
	}


	options {
		buildDiscarder(logRotator(numToKeepStr: '5'))
		disableConcurrentBuilds()
	}

	stages {
		stage('Build') {
			steps {
				sh 'jekyll build'
			}
		}

		stage('Publish') {
			steps {
				withCredentials([sshUserPrivateKey(credentialsId: 'jekyll-deploy-key', keyFileVariable: 'sshKeyFile')]) {
				    sh 'mkdir -p /root/.ssh'
		                    sh 'cp '+ sshKeyFile +' /root/.ssh/id_rsa'
                		    sh 'echo host repo.jeroensteenbeeke.nl > /root/.ssh/config'
		                    sh 'echo "\tStrictHostKeyChecking no" >> /root/.ssh/config'
		                    sh 'chmod 0400 /root/.ssh/config'
				    sh 'rsync -r _site/ deploy@23.94.72.114:/home/deploy/_site/'
				}

			}
		}
	}
}
