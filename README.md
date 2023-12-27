Welcome to Matt Nevers' ansible project!

Playbook Overview

This project utilizes passwordless ssh keys with a svc user with NOPASSWD configured sudoers file to enable a highly automatable enviornment. 
Ansible features such as tasks, roles, host_vars, tags, file, service managment, conditonals, lineinfile editing and more are all showcased here.

dist_upgrade.yml: This playbook for Debian/Ubuntu OS systems updates cache and runs dist upgrade on all hosts in
inventory file. If an upgrade was proccessed it will register a changed state and reboot those specific systems 
that require a reboot

server.yml: Playbook for general server administration tasks for any kind of server web,db or otherwise etc. 
Creates "svc" service user and sets up ssh key and sudoers file so passwordless ansible automation tasks can be performed

setup_apache.yml: For Debian/Ubuntu OS this package installs apache2 and php support on web servers group
and pushes template index.html file

web_role.yml: Rewrite of setup_apache.yml utilizing roles and variables

remove_apache.yml: Uninstalls apache and php support
