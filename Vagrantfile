# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  #config.vm.box = "debian/jessie64"
  config.vm.box = "debian/stretch64"

  # heplify
  config.vm.define "heplify-dev" do |heplify|
    heplify.vm.hostname = "heplify-dev"
    heplify.vm.network :private_network, ip: "10.1.0.224"
    heplify.vm.network :private_network, ip: "10.1.1.224"
  end

  config.vm.provider :virtualbox do |vb|
    vb.customize ["modifyvm", :id, "--memory", 512]
    vb.customize ["modifyvm", :id, "--cpus", 1]
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "tests/main.yml"
  end

  config.vm.provider "virtualbox" do |vb|
    vb.gui = false
    vb.name = "heplify-dev"
  end
end
