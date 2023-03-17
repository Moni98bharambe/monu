pipeline {
	agent {
		label "slave-1"
			}
		stages {
				stage ("this is stage-1") {
					steps {
						
						sh "yum install docker -y"
						sh "systemctl start docker"
						sh "docker run -itdp 80:80 --name server httpd"
						sh "docker cp index.html server:/usr/local/apache2/htdocs"
				}

			}		
	
		}
 }		
			
	
	
	
	
	
	
	
	
