# learn-devops   Date:  12-Feb-2021

firewalld in Centos  (iptables old version)
It is  software firewall 
Firewall is a way to filter or Prevent unwanted / unauthorized packets coming from outside the network into our network.

Step-1  install auto compilation shell in centos7

 yum install bash-completion bash-completion-extras

Step-2   Compile shell
	
	source /usr/share/bash-completion/bash_completion

Step-3  test  / compile shell
		
		firewall-cmd  --list-all-zones | less
Step-4 check active zone with brief information

		firewall-cmd --list-all
-------------------------------------------------------------------------------
    tar cfpz mydata_etc.tar.gz --exclude=/etc/yum.repos.d   /etc/
 
   tar  -tf  mydata_etc.tar.gz |  less
   tar cfpz mydata_etc.tar.gz --exclude=/etc/yum*   /etc/
  tar  -tf  mydata_etc.tar.gz |  less
systemctl strart  firewalld
   systemctl start  firewalld
  systemctl enable firewalld

----------------------------------------------------------------------------------


To Check Virtualization on Base machine 

Step-1  boot with Live USB then ;

Step-2 and open terminal and use following command wheather your CPU support virtualization or  not ?

	cat  /proc/cpuinfo   |   grep lm

  	cat  /proc/cpuinfo   |   grep vme

	cat  /proc/cpuinfo   |   grep vmx

------------------------------------------------------------------------------ 

