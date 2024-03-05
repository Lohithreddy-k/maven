piprline{ 
	agent any
	stages{
		stage{
			steps("scm"){
				git "https://github.com/Lohithreddy-k/maven.git"
				git branch: 'feature', url: 'https://github.com/Lohithreddy-k/maven.git'
				}
			}
		stage{
			steps("run"){
				sh "mvn clean install"
				sh "sh demo.sh"
				}
			}
		}
	}
