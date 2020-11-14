# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "centos/8"
  config.vm.box_version = "1905.1"
  config.vm.base_address = "192.168.1.253"
  config.vm.synced_folder "./", "/opt/vagrant", type: "rsync"

  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "provision/playbook.yml"
  end

end
