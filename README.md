# vagrant-smartos-gas: a Vagrant box with SmartOS + GNU assembler

# VAGRANT CLOUD

https://app.vagrantup.com/mcandre/boxes/vagrant-smartos-gas

# EXAMPLE

```console
$ cd test
$ vagrant up
$ vagrant ssh -c "cd /opt/vagrant && as -o hello.o && ld -o hello hello.o && ./hello"
Hello World!
```

# RUNTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider

## Recommended

* [vagrant-rsync-back](https://github.com/smerrill/vagrant-rsync-back) assists in copying artifacts from the guest to the host

# BUILDTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider
* [make](https://www.gnu.org/software/make/)

# EXPORT

```console
$ make vagrant-smartos-gas.box
```
