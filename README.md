You have to change passwords in hosts 

sudo ansible-playbook fedora-desktop.yml -i inventories/localhost/hosts

ansible-playbook -vvvvv create-keys.yml -i inventories/localhost/hosts

ansible-playbook upload-keys.yml -i hosts

ansible-playbook servers_env.yml -i hosts


