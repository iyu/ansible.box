# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "centos65"
  config.vm.box_url = "https://github.com/2creatives/vagrant-centos/releases/download/v6.5.3/centos65-x86_64-20140116.box"

  config.vm.define :node do |node|
    node.vm.network :private_network, ip: "192.168.33.10"
    node.vm.provision :ansible do |ansible|
      ansible.limit = "node"
      ansible.inventory_path = "inventory"
      ansible.playbook = "playbook.yml"
    end
  end

  config.ssh.insert_key = false

end
