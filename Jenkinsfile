//his is Jenkins file

pipeline {
	agent {
		label "built-in"
	}
		stages {
			stage ("23Q3") {
				steps {
					sh "cd /mnt/assignment"
					sh "git checkout 23Q3"
					sh "sudo docker run -itdp 8081:80 --name 23Q3 httpd"
					sh "sudo docker cp index.html 23Q3:/usr/local/apache2/htdocs"
			}
		}			
	}
}
