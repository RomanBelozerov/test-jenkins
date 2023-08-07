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
					sh "cp /var/lib/jenkins/workspace/Makefile.local Makefile.local"
					sh "printenv"
					sh "cat Makefile.local"
					sh "pwd"
					sh "ls -a"
					sh "cat Makefile.local"
				}
			}
		}
	}
}
