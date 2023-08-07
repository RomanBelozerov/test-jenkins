pipeline {
	
	agent {
		label "base"
	}
	
	stages {
		stage("Test jenkisfile") {
			steps {
				script {
					echo "Test jenkinsfile"
					sh "printenv"
					sh "pwd"
					sh "ls -a"
				}
			}
		}
	}
}
