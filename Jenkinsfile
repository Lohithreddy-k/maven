pipeline{ 
	agent any
	stages{
		stage("scm"){
			steps{
				git "https://github.com/Lohithreddy-k/maven.git"
				git branch: 'feature', url: 'https://github.com/Lohithreddy-k/maven.git'
				}
			}
		stage("run"){
			steps{
				sh "mvn clean install"
				sh "sh demo.sh"
				}
			}
		}
	}
