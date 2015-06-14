# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.network "forwarded_port", guest: 80, host: 8080

  config.omnibus.chef_version = :latest

  config.vm.provision "chef_zero" do |chef|
    chef.add_recipe "nginx"
  end
  
end
