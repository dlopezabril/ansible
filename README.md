# Ansible Automation Projects

# Set environment
source ~/Workspace/ansible-sernow/env/bin/activate
pip3 install ansible

# Set Path
cd ~/Workspaces/ansible-sernow

# Ping over an IP
ansible -i commands/inventory -m ping -u vagrant 10.42.0.15 --private-key=~/Workspaces/vagrant/centos7/.vagrant/machines/default/virtualbox/private_key

# ansible copy file in an host
ansible-playbook commands/copy_playbook.yml -i commands/inventory --private-key=~/Workspaces/vagrant/centos7/.vagrant/machines/default/virtualbox/private_key -vvvv

# ansible modify file in an host
ansible-playbook commands/modify_file_playbook.yml -i commands/inventory --private-key=~/Workspaces/vagrant/centos7/.vagrant/machines/default/virtualbox/private_key -vvvv

# ansible modify file in an host
ansible-playbook commands/osversions_playbook.yml -i commands/inventory --private-key=~/Workspaces/vagrant/centos7/.vagrant/machines/default/virtualbox/private_key -vvvv

# Video
~/videotutoriales/Systems/Ansible/ansible_howtouse.mp4