
   1.How to Install Jenkins in Ubuntu ?
   
    A.Admin to login root privelligance 
	 $ sudo su
	 
	B.Update your local package index
	$  apt update
	
	C.Install Java 
	$ apt install openjdk-11-jdk
	
	D.Install Jenkins Debian Packages
	 # This is the Debian package repository of Jenkins to automate installation and upgrade. To use this repository, first add the key to your system (for the Weekly Release Line):
	 $ sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
    https://pkg.jenkins.io/debian-stable/jenkins.io-2023.keysu
	
	Then add a Jenkins apt repository entry:
	E.echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
    https://pkg.jenkins.io/debian binary/ | sudo tee \
    /etc/apt/sources.list.d/jenkins.list > /dev/null
	
	  $ pwd (location check)
	  
	
    F.Update your local package index
	$ apt update
	
	G.then finally install Jenkins
     apt-get install jenkins
	 
	H.Jenkins server start or not
	 systemctl start jenkins
     systemctl status jenkins
	 
   J.firewall port 
    ufw allow 8080
    sudo ufw status
  
   I.How can you path idenification key in password into Console 
     cat  /var/lib/jenkins/secrets/initialAdminPassword
	 Administrator password: 
                             3e788bfa1ccf46ca8079c0c2dbbc0a30


  

	