# soninjas.drush
Ansible role to install composer and drush

#Sample centos playbook file:
--------------

    hosts: centos-webserver
    remote_user: ansible
    become: true
    
    vars_files:
      - "../roles/soninjas.drush/vars/main.yml"
      - "../roles/soninjas.drush/tasks/drush.yml"

    roles:
       - role: soninjas.drush
         tags: drush

## Role Variables
--------------

You can change variables `vars/main.yml` . You are free to change any part of the role and adapt it to your needs

## Author Information
------------------
Southern Oregon Net Ninjas
