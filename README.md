# ELK - Installtion of ELK on the Cent OS 7 
These roles works butter smooth with the VM instances of GCP. 
I cloned the git repo of the ELK on my GCP VM and then ran runsetup.yaml. For GCP instances you need to install git/ansible. Also, will need to edit /etc/ssh/sshd_config in order to enable password authentication. By default GCP instances uses only file based authentication. 
User named Kunal has also been created on client machines which also has permission to do sudo su

I have used two roles in runsetup.yaml you can use filebeat role seperately. 
```
# yum install ansible git 
# ansible-playbook runsetup.yaml -i elk_hosts
```

