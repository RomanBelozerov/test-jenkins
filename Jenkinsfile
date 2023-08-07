pipeline {
	
	agent {
		label "base"
	}
	
	stages {
		stage("Test jenkisfile") {
			steps {
				script {
					echo "Test jenkinsfile"
					echo 'envoy-docker-build' >> Makefile.local
					sh "printenv"
					sh "cat Makefile.local"
					sh "pwd"
					sh "ls -a"
				}
			}
		}
	}
}
