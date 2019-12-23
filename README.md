# k8s-vagrant-ansible


## Set up

Install latest version of ansible.
```
python3 -m pip install -U ansible
```
virtualbox and vagrant can be installed from the following links:
https://www.virtualbox.org/wiki/Downloads
https://www.vagrantup.com/downloads.html

update /etc/hosts file to include the following:
      192.168.120.11 node1
      192.168.120.12 node2
      192.168.120.13 node3

Run the following to create cluster of VMs.
```
vagrant up
vagrant status
ssh vagrant@node1
ssh vagrant@node2
```
You can easily destroy the cluster by:
```
vagrant halt
vagrant destroy
```
