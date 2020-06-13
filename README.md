# 1. vagrant-virtualbox
Provisioning Virtual Machine with Vagrant

Ref: https://www.lukmanlab.com/tag/vagrant/

- [1. vagrant-virtualbox](#1-vagrant-virtualbox)
  - [1.1. Run this Vagrantfile](#11-run-this-vagrantfile)
  - [1.2. Basic Command Vagrant](#12-basic-command-vagrant)
    - [1.2.1. Initialization Vagrantfile](#121-initialization-vagrantfile)
    - [1.2.2. Running Vagrantfile (Provisioning)](#122-running-vagrantfile-provisioning)
    - [1.2.3. Add Boxes to Local](#123-add-boxes-to-local)
    - [1.2.4. Check Status Vagrantfile](#124-check-status-vagrantfile)
    - [1.2.5. Distroy VM Provisioned](#125-distroy-vm-provisioned)
    - [1.2.6. SSH to VMs](#126-ssh-to-vms)
    - [1.2.7. Save State to Snapshot VM](#127-save-state-to-snapshot-vm)
    - [1.2.8. Restore State Snapshot](#128-restore-state-snapshot)

## 1.1. Run this Vagrantfile
```
git clone https://github.com/lukmanlab/vagrant-virtualbox.git
cd vagrant-virtualbox
vagrant up
```

## 1.2. Basic Command Vagrant

### 1.2.1. Initialization Vagrantfile
`$ vagrant init hashicorp/precise64`

### 1.2.2. Running Vagrantfile (Provisioning)
`$ vagrant up`

### 1.2.3. Add Boxes to Local
`$ vagrant box add ubuntu/xenial64`

List boxes downloaded (~/.vagrant.d/boxes/): 
`$ vagrant box list`

Update to Latest Version:
`$ vagrant box update`

### 1.2.4. Check Status Vagrantfile
`$ vagrant status`

List Boxes Provisioned:
`$ vagrant global-status`

### 1.2.5. Distroy VM Provisioned
`$ vagrant destroy`

### 1.2.6. SSH to VMs
`$ vagrant ssh node1`

### 1.2.7. Save State to Snapshot VM
`$ vagrant snapshot save node1 masih-fresh`

### 1.2.8. Restore State Snapshot
`$ vagrant snapshot restore node1 masih-fresh`