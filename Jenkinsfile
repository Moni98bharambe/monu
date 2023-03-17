pipeline {
	agent {
		label "slave-1"
			}
		stages {
				stage ("this is stage-1") {
					steps {
						
						sh "sudo yum install docker -y"
						sh "sudo systemctl start docker"
						sh "sudo docker run -itdp 80:80 --name server httpd"
						sh "sudo docker cp index.html server:/usr/local/apache2/htdocs"
				}

			}		
	
		}
 }		
			
	
	
	
	
	
	
	
	
