# Learning repo for Ansible

### Test ping
ansible all -m ping -i /inventory/inv.yml

### Test first playbook
ansible-playbook -i /inventory/inv.yml /playbooks/aptupdate.yml

