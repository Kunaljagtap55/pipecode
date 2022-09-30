pipeline {
           agent { label 'slave3' }
		    
			stages {
			      stage ('install apache'){
				  
				  steps {sh "sudo yum install httpd -y"}
				  }
				  
				  stage ('start apache'){
				  
				  steps {sh "sudo service httpd start"
				  sh "sudo chkconfig httpd on"}
				  
				  }
				  stage ('file deploy'){
				  steps {
				           
                            sh "cp -r /mnt/index.html /var/www/html"
						   sh " chmod -R 777 /var/www/html "

}				  
				  }
				  }
				  
			}
		   

