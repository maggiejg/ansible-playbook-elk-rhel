# Ansible Playbook for ELK on RHEL
 
This playbook is for setting up version 6.x of the ELK Stack on a remote server. 

## Notes and requirements
 - The playbook was built and tested on RHEL EC2 instances, for ELK versions 6.x 
 - You will need Ansible installed and running
 - Playbook is currently configured to set up the ELK stack together 
 - Due to size constraints for this demo, Logstash, Metricbeat for perfomance monitoring and Filebeat are available as roles, but have not been added. This can be changed in your site.yml file by adding the roles.
 
 
 ## Instructions
 
 1. Edit your Ansible hosts file ('/etc/ansible/hosts') and add an 'elkservers' entry for the server you wish to install ELK on. You can of course name the host any way you want, this is just an example. 
 2. Verify connectivity to the ELK server.
 3. In the terminal on the machine hosting Ansible, clone this repo.
 4. Cd into the directory, and run:
 `ansible-playbook site.yml`
 
 The plays in the playbook will run on the target server, installing ELK. 
 
[site.yml]: https://github.com/maggiejg/ansible-playbook-elk-rhel.git
