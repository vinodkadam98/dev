pipeline {
        agent {
          label {
           label "built-in"
		   customWorkspace "/mnt/pipeline"
}
}
         stages {
           stage ("stage-1") {
		   steps {
		          sh "yum install httpd -y"
				  sh "service httpd start"
				 sh "cp -r index.html /var/www/html"
				  sh "chmod -R 777 /var/www/html/index.html"
			          sh "yum install tree -y"
		   }
		   }

}
}
