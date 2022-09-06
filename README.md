# Tools Box

A set of Infrastructure-as-code (IaC) scripts. This ranges from a local virtual machine with Vagrant
to a virtual machine on a cloud service provider's platform. While a local VM box will grant student
full permission the cloud VM access should be limited and short-live. Both platforms will have the
same OS, Ubuntu, and will be pre-installed with same set of softwares (tools used in the class).

The primary reason is to provide student with alternative to the EECS school's Linux server. This
tool should solve the following situations

- System administrator is still on a vacation on the first week of the semester.
- Students do not have access to the EECS school's Linux server during a quiz or an exam (no account created
  forget username and/or password).
- (theoretical) A sanboxed environment to safely run students' souce code. It is theoretical
  because the isolation is not tested.

## Create a local virtual machine via Vagrant

A Vagrantfile to create a VM with most tools in this class.

### Usage

First, make sure that you have HashiCorp's Vagrant installed [https://www.vagrantup.com/](https://www.vagrantup.com/). You will also need VirtualBox which can be installed from [https://www.virtualbox.org/](https://www.virtualbox.org/).

Clone this repository and run `vagrant up`

```console
git clone https://github.com/OU-CS3560/tools-box.git
cd tools-box/vagrant-box
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
## Create a cloud-based virtual machine

TBA