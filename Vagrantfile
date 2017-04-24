Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.provision :ansible do |ansible|
    ansible.playbook = "vagrant.yml"
  end

  config.vm.provider "virtualbox" do |v|
    v.memory = 1024
  end

  config.vm.network "private_network", type: "dhcp"
end
