## Adding the ansible repo in the ubuntu

sudo apt-add-repository ppa:ansible/ansible

sudo apt update

sudo apt-get install ansible

### hosts file configuration inside (/etc/ansible/hosts)

[servers]
server1 ansible_host=3.70.241.8
server2 ansible_host=3.71.174.252
server1 ansible_user=ubuntu
server2 ansible_user=ec2-user

[all:vars]
ansible_python_interpreter=/usr/bin/python3
ansible_ssh_private_key_file=/home/ubuntu/keys/amazon.pem
