# odoo-ansible-installer
Automated process for Odoo Deployment in cloud stack mode, using ansible

This installer depends on the following Ansible Roles:
  - sebalix.odoo, 1.2.1
  - azavea.postgresql, 0.4.0
  - jdauphant.nginx, v2.6 
  - dresden-weekly.network-interfaces, 1.0

To install the required Ansible Roles, you must issue the following commmand:
    `ansible-galaxy install <role-name>`

To run this installer, you must use:
    `ansible-playbook --flush-cache -i hosts stack-setup.yml`


Please check the variables.yml file for custom configurations, and the hosts
file for initial server node list
