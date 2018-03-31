# Hello Ansible

This is a sample setup with Ansible for consifuration management and orchestration.

Setup includes Ansible scripts to build a 3-tiered web application environment leveraging NGINX, Apache2, Python, and MySQL on Ubuntu Linux servers.

This project includes sample Ansible scripts for engineers interested in configuration management, orchestration, infrastructure-as-code, and devops principles. This is the code for mastering ansible tutorial on Udemy.

## Sample Ansible Scripts
* Ansible configuration playbooks to deploy a 3-tier web application
* Ansible roles with tasks, handlers, files, templates, and default variables
* Operational playbooks to check cluster status and perform a cluster restart.
* Optimized Ansible playbooks to reduce playbook execution time.

## Optimization
 
- Look for the places that doe snot need gathering facts
 ```gather_facts: false```
- Implement cache valid time and skip unnecessary cache validation 
- Limit execution by host: when you run the playbooks, you can limit the execution to some subset of the hosts
  ```ansible-playbook playbooks/site.yml --limit node2```
- Limit execution by tasks using tags.

## Resources
- Fist place to start (my opinion): https://www.ansible.com/resources/get-started
- You perefer to follow an instructor: https://www.udemy.com/mastering-ansible/
