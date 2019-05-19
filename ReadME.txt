CS 312 HW 7 manual
Group Members: Lizz Premer, Jacob Dugan, Haofeng Tian, Miao Zhou

File Name
	Script: hw7.sh
	Playbook: webserver.yaml
 

Instructions:
	1. Start the pfSense_Reference VM
	
	2. Wait until router VM is up
	
	3. Start the CentOS_CLI_Reference VM
	
	4. Start 4 Alpine_Reference VMs
	
	5. In each Alpine VM, use command ‘ip addr’ to retrieve IP addresses.
	
	6.Download all 4 files we need by order:
	  curl https://raw.githubusercontent.com/Duganja/CS312_HW7/master/ansible-index.html > ~/ansible-index.html
	  curl https://raw.githubusercontent.com/Duganja/CS312_HW7/master/hosts.ini > ~/hosts.ini
	  curl https://raw.githubusercontent.com/Duganja/CS312_HW7/master/hw7.sh > ~/hw7.sh
	  curl https://raw.githubusercontent.com/Duganja/CS312_HW7/master/webserver.yaml > ~/webserver.yaml

	  Make sure the CentOS VM has the “hw7.sh”, “ansible-index.html”, “webserver.yaml” file, and the “hosts.ini” files.
	
	7. Run the “sh hw7.sh” command
	
	8. The script will prompt for creating the ssh key, press enter on these three prompts so it gets default values. If there are 		   already keys generated, you will also have to enter “y” once
	
	9. Enter the IP addresses of the four Alpine VMs
	
	10. You will have to enter the passwords for the four Alpine VMs, you may also have to enter “yes” if it is the first time 		    running the script.
	
	11. If at any point the Alpine VM’s IP addresses change after running the script once, the hosts.ini will need to be reset.


Additional files:
	Host file: hosts.ini
	HTML file: ansible-index.html
