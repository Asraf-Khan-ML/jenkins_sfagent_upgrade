##Ansible script to upgrade sfagent for Multiple Hosts

ansible.cfg - Ansible configuration file.

hosts - Ansible Inventory File

playbooks - Its a directory holds all playbooks.

Requirement: 

	1. install ansible 
    
    2. copy node ssh key to local machine and change permission with chmod 400  <ssh key>
	
	3. Update nodes details to upgrade sfagent in host file.

Execution:

	ansible-playbook upgrade_sfagent_vm.yml --key-file=<path to ssh key file>  -b -v

	Example
		ansible-playbook upgrade_sfagent_vm.yml --key-file=/home/centos/user-qa-aws-ssh.pem -b -v
