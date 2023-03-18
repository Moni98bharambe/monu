pipeline {
	agent {
		label {
			label "built-in"
			customWorkspace "/mnt/project"
		}
		}
		stages {
			stage ("copy-git-index-file") {
				steps {
					sh "rm -rf /var/lib/docker/volumes/vol1/_data/index.html"
					sh "cp /mnt/project/index.html /var/lib/docker/volumes/vol1/_data/"	
				}
			}
			stage ("install docker") {
				steps {
					sh "docker run -itdp 81:80 -v vol1:/usr/local/apache2/htdocs/ --name siya httpd"
					
			}
			
		}
	
	}


}	
			
			
	
	
	
	
	
	
	
