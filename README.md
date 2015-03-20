ANSIBLE BOX
====
https://atlas.hashicorp.com/iyu/ansible

## Installation for Mac

### Vagrant
http://www.vagrantup.com/downloads.html

### Virtualbox
https://www.virtualbox.org/wiki/Downloads

### Ansible
```sh
$ brew install ansible
```

## Usage

### Basic
```sh
$ vagrant up
$ ansible-playbook -i inventory --ask-sudo-pass playbook.yml
$ vagrant package
```
https://atlas.hashicorp.com/iyu/boxes/ansible/versions/new

### Update
```sh
$ vagrant destroy
$ vim playbook.yml # edit playbook.yml
$ vagrant up
$ ansible-playbook -i inventory --ask-sudo-pass playbook.yml
$ vagrant package
```
https://atlas.hashicorp.com/iyu/boxes/ansible/versions/new
