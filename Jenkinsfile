pipeline {
	agent any
	stages{
		stage("clone or remove the github project")
		{
			steps{
				sh "sudo rm -rf /home/shahzebalam/github"
				sh "cd /home/shahzebalam/"
				sh "sudo mkdir -p /home/shahzebalam/github"
				sh "sudo git clone https://github.com/shahzebalam999/test.git /home/shahzebalam/github"
			
			}
		}
	
	
			stage("changing the permission"){
			steps {
				sh "chown -R jenkins:jenkins /home/shahzebalam/github/test"
			}
		}
	
	}
	
}
