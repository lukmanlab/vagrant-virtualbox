Vagrant.configure("2") do |config|
  config.vm.define :node1 do |node1|
    node1.vm.box = "ubuntu/xenial64"
    node1.vm.network "private_network", ip: "192.168.50.4"
    node1.vm.define "node1"
    node1.vm.hostname = "node1"
  
    node1.vm.provider "virtualbox" do |vb|
      vb.name = "Ubuntu-Vagrant16.04"
      vb.cpus = 1
      vb.memory = 1024
    end
  end

  config.vm.define :node2 do |node2|
    node2.vm.box = "ubuntu/bionic64"
    node2.vm.network "private_network", ip: "192.168.50.5"
    node2.vm.define "node2"
    node2.vm.hostname = "node2"
  
    node2.vm.provider "virtualbox" do |vb|
      vb.name = "Ubuntu-Vagrant18.04"
      vb.cpus = 2
      vb.memory = 1024
    end
  end
end

# VAGRANTFILE_API_VERSION = "2"
 
# Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
#   config.vm.box = "ubuntu/bionic64"
#   config.vm.network "private_network", ip: "192.168.50.5"
#   config.vm.define "node2"
#   config.vm.hostname = "node2"

#   config.vm.provider "virtualbox" do |vb|
#     vb.name = "Ubuntu-Vagrant18.04"
#     vb.cpus = 2
#     vb.memory = 1024
#   end
# end