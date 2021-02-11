# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/focal64"
    config.vm.synced_folder "./", "/bootstrap"
    config.vm.provider "virtualbox" do |vb|
      vb.gui = true
      vb.memory = "4096"
    end
  
    config.vm.provision "shell", inline: <<-SHELL
      sudo apt-get update && sudo apt-get install ubuntu-desktop python3 -y
    SHELL
  
    config.vm.provision "ansible" do |ansible|
      ansible.verbose = "v"
      ansible.galaxy_role_file = "bootstrap/requirements.yml"
      ansible.galaxy_roles_path = "bootstrap/roles/"
      ansible.playbook = "bootstrap/vagrant.yaml"
      ansible.raw_arguments = ["--diff"]
    end
  end