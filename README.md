# ansible
Ansible Automation Projects

> **Access to Ansible workspace**
```shell
code ~/Workspaces/ansible/ansible.code-workspace
```

> **Set python source**
```shell
source ~/Workspaces/splunk_scripts/env/bin/activate
```

> **Set Path**
```shell
cd ~/Workspaces/ansible
```

> **ansible copy file in an host**
```shell
ansible-playbook commands/copy_playbook.yml -i commands/inventory --private-key=~/Workspaces/vagrant/centos7/.vagrant/machines/default/virtualbox/private_key -vvvv
```

> **ansible modify file in an host**
```shell
ansible-playbook commands/modify_file_playbook.yml -i commands/inventory --private-key=~/Workspaces/vagrant/centos7/.vagrant/machines/default/virtualbox/private_key -vvvv
```

> **ansible modify file in an host**
```shell
ansible-playbook commands/osversions_playbook.yml -i commands/inventory --private-key=~/Workspaces/vagrant/centos7/.vagrant/machines/default/virtualbox/private_key -vvvv
```

> **Ping over an IP**
```shell
ansible -i commands/inventory -m ping -u vagrant 10.42.0.15 --private-key=~/Workspaces/vagrant/centos7/.vagrant/machines/default/virtualbox/private_key
```

> **Projects**
> [ansible_copy.zip](:storage/4ceba4ea-10fa-4f24-9734-f2547cd27107/09b971b3.zip)

> **Video:** 
> ~/videotutoriales/Systems/Ansible/ansible_howtouse.mp4