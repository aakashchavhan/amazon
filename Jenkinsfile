pipeline{
	agent {
		label {
			label "built-in"
			customWorkspace "/data/pipeline"
				}
				}

		stages {
			stage ('install-apache-server') {
				steps {
					sh "yum install httpd -y"	
						}
											}
			stage ('deploy-index.html') {
				steps {
					sh "cp -r index.html /var/www/html"
					sh "chmod -R 777 /var/www/html/index.html"
						}
											}
			stage ('restart apacher-server') {
				steps {
					sh "service httpd restart"	
						}
											}
			
			}
		}
