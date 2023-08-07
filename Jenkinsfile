pipeline {
	
	agent {
		label "base"
	}
	
	stages {
		stage("Test jenkisfile") {
			steps {
				script {
					echo "Test jenkinsfile"
					echo -e "BUILD_DIR := /var/lib/jenkins/workspace/envoy-docker-build\nLLVM_ROOT := /usr/lib/llvm-15\nWRAPPERS_DIR := /var/lib/jenkins/workspace/fakecc" > Makefile.local
					sh "printenv"
					sh "pwd"
					sh "ls -a"
				}
			}
		}
	}
}
