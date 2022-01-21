# jenkins
Jenkins and maven installaion command on linux EC2 
How to Install Jenkins on AWS EC2 Instance?

#use these commands to install jenkins in the following given sequence.

---------------------------------------------------------------------------

> sudo amazon-linux-extras install epel -y

> sudo yum update –y

> sudo wget -O /etc/yum.repos.d/jenkins.repo \
    https://pkg.jenkins.io/redhat-stable/jenkins.repo
    
> sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key

> sudo yum upgrade

> sudo yum install jenkins java-1.8.0-openjdk-devel -y

> sudo systemctl daemon-reload

> sudo systemctl start jenkins

> sudo systemctl status jenkins

-------------------------------------------------------------


# if you faced any issues while unlocking Jenkins, then use the command:

> sudo cat /var/lib/jenkins/secrets/initialAdminPassword


--------------------------------------------------------------

Maven installation

> yum installl maven -y

--------------------------------------------------------------

#use this command to find JAVA_HOME path:

> java -XshowSettings:properties -version 2>&1 > /dev/null | grep 'java.home'

-----------------------------------------------------------------
