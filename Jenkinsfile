pipeline {
	
	agent {
		label "base"
	}
	
	stages {
		stage("Test jenkisfile") {
			steps {
				script {
					echo "Test jenkinsfile"
					echo "BUILD_DIR := /var/lib/jenkins/workspace/envoy-docker-build" > Makefile.local
					echo "LLVM_ROOT := /usr/lib/llvm-15" >> Makefile.local
					echo "WRAPPERS_DIR := /var/lib/jenkins/workspace/fakecc" >> Makefile.local
					sh "printenv"
					sh "cat Makefile.local"
					sh "pwd"
					sh "ls -a"
				}
			}
		}
	}
}
