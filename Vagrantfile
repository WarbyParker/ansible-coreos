# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "yungsang/coreos"
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = 'playbook.yml'
    ansible.groups = {
      "coreos" => ["default"],
    }
  end
end
