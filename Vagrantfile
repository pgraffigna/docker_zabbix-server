# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.ssh.insert_key = false
  config.vm.synced_folder ".", "/vagrant", disabled: true

  config.vm.define "zabbix-server" do |z|
    z.vm.box = "geerlingguy/ubuntu1804"
    z.vm.network "public_network"
    z.vm.hostname = "zabbix-server"
    z.vm.provision :docker
    z.vm.provision :docker_compose
  end

  config.vm.provider :virtualbox do |vbox|
    vbox.name = "zabbix-server"
    vbox.memory = 4096
    vbox.cpus = 2
    vbox.check_guest_additions = false
  end
end


