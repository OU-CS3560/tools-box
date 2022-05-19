# Tools Box

A Vagrantfile to create a VM with most tools in this class.

## Setup

First, make sure that you have HashiCorp's Vagrant installed [https://www.vagrantup.com/](https://www.vagrantup.com/). You will also need VirtualBox which can be installed from [https://www.virtualbox.org/](https://www.virtualbox.org/).

Clone this repository and run `vagrant up`

```console
git clone https://github.com/OU-CS3560/tools-box.git
cd tools-box
vagrant up
```

A virtual machine will be created and provisioned for you. To obtain a shell of the VM you can run

```console
vagrant ssh
```

To exit out of the VM shell session, `exit` or `logout` can be used. Keep in mind that the VM will still be running, and to properly stop it you can run

```console
vagrant suspend
```

Or to complete poweroff the VM, run

```console
vagrant halt
```

To remove the VM, run

```console
vagrant destroy
```
