Welcome to Matt Nevers' ansible project!

Playbook Overview

This project utilizes passwordless ssh keys with a svc user with NOPASSWD ALL:ALL configured sudoers file to enable a highly automatable enviornment. 

dist_upgrade.yml: This playbook for Debian/Ubuntu OS systems updates cache and runs dist upgrade on all hosts in
inventory file. If an upgrade was proccessed it will register a changed state and reboot those specific systems 
that require a reboot

setup_apache.yml: For Debian/Ubuntu OS this package installs apache2 and php support on web servers group
and pushes template index.html file

remove_apache.yml: Uninstalls apache and php support
