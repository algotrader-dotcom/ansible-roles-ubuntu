# -*- mode: ruby -*-
Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-16.04"

  config.vm.network "forwarded_port", guest: 2222, host: 22
  config.vm.network "forwarded_port", guest: 80, host: 80
  config.vm.network "forwarded_port", guest: 8983, host: 8983

  config.vm.network "private_network", ip: "192.168.30.10"

  config.vm.provider "virtualbox" do |vb|
      vb.memory = "2048"
  end
end
