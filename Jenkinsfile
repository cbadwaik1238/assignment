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
					sh "docker run -itdp 8081:80 --name 23Q3 httpd"
					sh "docker exec -it 23Q3 bash"
					sh "cd htdocs"
					sh "chmod 777 index.html"
					sh "docker cp index.html 23Q3:/usr/local/apache2/htdocs"
			}
		}			
	}
}
