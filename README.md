# Vagrant Test Application

Test application to mess around with provisioning containers with Vagrant and Ansible.

## Prerequisites
- [Vagrant](https://www.vagrantup.com/downloads) must be installed (see `./installs`)
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads) must be installed (see `./installs`)
- [Hyper-V must be disabled](https://docs.microsoft.com/en-us/troubleshoot/windows-client/application-management/virtualization-apps-not-work-with-hyper-v)
- The [guest ansible](https://github.com/vovimayhem/vagrant-guest_ansible) Vagrant plugin must be installed

## Vagrant Commands

To create and configure the virtual machine:
```
> vagrant up
```

To ssh into the virtual machine:
```
> vagrant ssh
```

To stop the virtual machine:
```
> vagrant halt
```

To destroy the virtual machine and associated resources:
```
> vagrant destroy
```

To connect to the virtual machine using SSH:
```
> vagrant ssh
```

Alternatively, to connect to the created user account using SSH:
```
> ssh -i <private-key> ajones@localhost -p 2222
```