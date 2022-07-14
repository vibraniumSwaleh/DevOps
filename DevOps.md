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
- Window powershell - Cross-platform task automation command-line shell. If you don't have it, you can get it from here [powershell](https://docs.microsoft.com/en-us/powershell/scripting/overview?view=powershell-7.2). 
- Visual Studio - [source code editor](https://visualstudio.microsoft.com/).

## Deploying VM

The VM deployed was a [bento/ubuntu-18.04](https://app.vagrantup.com/bento/boxes/ubuntu-18.04) with minimal configuration. Any box your choice can be used in this deployment. Vagrant has a list of boxes it supports but you can use your own custom ones if you so wish.

Open powershell and navigate to a folder (preferably an empty one) you want to have your box in. Then run the vagrant command below to setup your vagrant config file.
```
vagrant init
```
The config file can be openned in any text editor to make changes to the configurations. 
Here is the config file used:
```
Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-18.04"
end
```

Once you have the basic vagrant code in the file and save, jump onto your powershell and spin up your vm with a single line of command:
```
vagrant up
```
If you want to shutdown your vm then the command below will do it for you:
```
vagrant halt
```
and to delete all traces of your vagrant machine then the code below will do the magic:
```
vagrant destroy
```


