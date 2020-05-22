You have to change passwords in hosts 

sudo ansible-playbook fedora-desktop.yml -i inventories/localhost/hosts

ansible-playbook create-keys.yml -i inventories/localhost/hosts

ansible-playbook upload-keys.yml -i inventories/production-unsecure/hosts

ansible-playbook fedora-servers.yml -i inventories/production/hosts

ansible-playbook create-vpn.yml -i inventories/production/hosts

ssh -i .keys/*_id_rsa 


