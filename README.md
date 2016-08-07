# openstack-cloud single node setup procedure

Here we are going to deploy openstack on a single node, i.e all openstack components Nova, Glance, Keystone, Quantum and Horizon will be running in the same box. Nova-compute is also running on the same machine which will provision virtual machines on the KVM.

Requirements:

* Ubuntu 12.04 running on Oracle VirtualBox with two NIC ‘s.

* Setup a ubuntu virtual machine in virtualBox. 

* Add a second NIC to the VM.

* Power Off the Virtual Machine

* In the Network Section select Adapter 2 tab

* Select “Attached to:” to internal

* Power On the VM

* When the VM boots up configure to network for second NIC
  Edit /etc/network/interfaces to something like

* Restart Network service
  service networking restart

* You can verify your network setting using “ ifconfig ”
