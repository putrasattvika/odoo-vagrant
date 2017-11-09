# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "debian/jessie64"

  config.vm.hostname = "odoo.test"
  config.vm.network :private_network, ip: "192.168.100.33"

  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "provision/odoo.yml"
  end
end
