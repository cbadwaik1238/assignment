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
					sh "docker run -itdp 90:80 --name 23Q2 httpd"
					sh "docker exec -it 23Q2 bash"
					sh "cd htdocs"
					sh "chmod 777 index.html"
					sh "docker cp index.html 23Q2:/usr/local/apache2/htdocs"
			}
		}			
	}
}
