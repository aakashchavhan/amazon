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
