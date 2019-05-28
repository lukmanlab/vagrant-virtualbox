# vagrant-virtualbox
Provisioning Virtual Machine with Vagrant

Ref: https://www.lukmanlab.com/tag/vagrant/

## Basic Command Vagrant

### Initialization Vagrantfile
`$ vagrant init hashicorp/precise64`

### Running Vagrantfile (Provisioning)
`$ vagrant up`

### Add Boxes to Local
`$ vagrant box add ubuntu/xenial64`

List boxes downloaded (~/.vagrant.d/boxes/): 
`$ vagrant box list`

Update to Latest Version:
`$ vagrant box update`

### Check Status Vagrantfile
`$ vagrant status`

List Boxes Provisioned:
`$ vagrant global-status`

### Distroy VM Provisioned
`$ vagrant destroy`

### SSH to VMs
`$ vagrant ssh node1`
