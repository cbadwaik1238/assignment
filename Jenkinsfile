//this is Jenkins file

pipeline {
	agent {
		label "built-in"
	}
		stages {
			stage ("23Q2") {
				steps {
					sh "cd /mnt/assignment"
					sh "git checkout 23Q2"
					sh "sudo docker run -itdp 90:80 --name 23Q2 httpd"
					sh "sudo docker cp index.html 23Q2:/usr/local/apache2/htdocs"
			}
		}			
	}
}
