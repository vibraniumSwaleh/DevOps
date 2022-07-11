# DevOps

This is a demo on how to use [**vagrant**](https://www.vagrantup.com/) to deploy virtual machines. Vagrant is an open-source software tool for building and and maintaining portable virtual software development environments; e.g., for [VirtualBox](https://www.vagrantup.com/docs/providers/virtualbox), [Hyper-V](https://www.vagrantup.com/docs/providers/hyperv), [Docker containers](https://www.vagrantup.com/docs/providers/docker), [VMware](https://www.vagrantup.com/docs/providers/vmware), and [AWS](https://www.vagrantup.com/docs/plugins/providers) [AWS Github](https://github.com/mitchellh/vagrant-aws).

Vagrant has an easy to use workflow and allows for automation lowering development setup time. It uses a declarative configuration file which describes all your software requirements, packages, operating system configuration, users, and more.

Vagrant also integrates with your existing configuration management tooling like Ansible, Chef, Docker, Puppet or Salt, so you can use the same scripts to configure Vagrant as production.

## Enviroment

The demo was run in a windows 11 environment.

## Software

To deploy virtual machines for this demo in window 11, a number of tools were used to effect that. Below is the list of the software and tools used.

- Virtualbox - The provider used to deloy the virtual machines in. You can use provider of your choice and vagrant has documentation for different providers it supports. See this for more information [vagrant providers](https://www.vagrantup.com/docs/providers).
- Vagrant - The tool used to provision virtual machines using a configuration file. Download from [vagrant](https://www.vagrantup.com/downloads).
- Putty - Free open source software used to ssh into vitrual machines. Download from [Putty](https://www.putty.org/).
