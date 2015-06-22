# W2C3 Live CD Vagrant

## This is a Vagrant configuration for [pablobm/w2c3-livecd](https://github.com/pablobm/w2c3-livecd). 

### 1. Install the dependencies if you do not already have them

- VirtualBox ([Download Page](https://www.virtualbox.org/wiki/Downloads)]
- Vagrant ([Download Page](https://www.vagrantup.com/downloads))

### 2. Clone this repository into a directory
```bash
$ git clone git@github.com:madebydavid/w2c3-livecd-vagrant.git w2c3-livecd-vagrant
$ cd w2c3-livecd-vagrant
$ git submodule update --init --recursive
```

### 3. Install the base image and start the VM
```bash
$ vagrant box add "deb/jessie-amd64" https://vagrantcloud.com/deb/boxes/jessie-amd64/versions/2.0/providers/virtualbox.box --provider virtualbox
$ vagrant up
```

### 4. SSH to the VM and build
```bash
$ vagrant ssh

The programs included with the Debian GNU/Linux system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Debian GNU/Linux comes with ABSOLUTELY NO WARRANTY, to the extent
permitted by applicable law.
Last login: Tue Apr 28 20:06:09 2015 from 10.0.2.2
vagrant@jessie-amd64:~$ cd /vagrant/w2c3-livecd/
vagrant@jessie-amd64:/vagrant/w2c3-livecd$ sudo lb build
```

