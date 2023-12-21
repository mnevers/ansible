ansible all -m ping 
ansible-playbook --ask-become-pass book.yml
ansible all -m gather_facts --limit ip
ansible-playbook --tags none --ask-become-pass book.yml
ansible-playbook --tags "db,web" book.yml
