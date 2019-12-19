# SED-challenge
# prerequisites
* pip install awscli 
* aws configure 
  - enter keys
* grab the ami-id, subnet-id, security-group-id, and create key-pair and paste in playbook    
* Execute the ec2-provision playbook - ansible-playbook instance.yml
* grab the the dns - ansible group-name -m ec2_instance_facts & paste in the server configuration .conf file and also in the openssh-cli 
* Run apache playbook - ansible-playbook /etc/ansible/ec2.yml
* roles-stucture
  - tasks dir - main.yml has all tasks  
  - files dir - files to be copied to .conf and index file 
  - handlers dir - main.yml restarts the apache-server
