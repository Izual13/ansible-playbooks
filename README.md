You have to change passwords in hosts 

sudo ansible-playbook localhost_env.yml -i hosts

ansible-playbook servers_env.yml -i hosts

ansible-playbook create-keys.yml -i hosts

ansible-playbook upload-keys.yml -i hosts
