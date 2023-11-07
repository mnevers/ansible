ansible all -m ping 
ansible-playbook --ask-become-pass install_apache.yml
ansible all -m gather_facts --limit ip
