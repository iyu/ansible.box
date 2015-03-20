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
$ vagrant package --output boxes/package-{version}.box
```
> Bug exists in vagrant@1.7.1. @see https://github.com/mitchellh/vagrant/issues/4962

https://atlas.hashicorp.com/iyu/boxes/ansible/versions/new

### Update
```sh
$ vagrant destroy
$ vim playbook.yml # edit playbook.yml
$ vagrant up
$ vagrant package --output boxes/package-{version}.box
```
https://atlas.hashicorp.com/iyu/boxes/ansible/versions/new
