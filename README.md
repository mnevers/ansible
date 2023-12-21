Welcome to Matt Nevers' ansible project!

Playbook Overview

dist_upgrade.yml: This playbook for Debian/Ubuntu OS systems updates cache and runs dist upgrade on all hosts in
inventory file. If an upgrade was proccessed it will register a changed state and reboot those specific systems 
that require a reboot

setup_apache.yml: For Debian/Ubuntu OS this package installs apache2 and php support on web servers group
and pushes template index.html file

remove_apache.yml: Uninstalls apache and php support
