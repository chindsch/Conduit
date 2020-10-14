# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-20.04"
  config.vm.provision "shell", path: "provision.sh"
  config.vm.network "private_network", ip: "192.168.10.100"
  config.vm.network "forwarded_port", guest: 4100, host: 8080, id: "nginx"
end