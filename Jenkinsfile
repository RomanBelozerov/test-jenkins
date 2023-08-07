pipeline {
	
	agent {
		label "base"
	}
	
	stages {
		stage("Test jenkisfile") {
			steps {
				script {
					echo "Test jenkinsfile"
					sh "ls -a"
					sh "echo 'BUILD_DIR := /var/lib/jenkins/workspace/envoy-docker-build' >> Makefile.local"
					sh "cat Makefile.local"
					sh "pwd"
					sh "ls -a"
				}
			}
		}
	}
}
