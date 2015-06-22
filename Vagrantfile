# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

    config.vm.box = "deb/jessie-amd64" 

    config.vm.provision :shell, :path => "bootstrap.sh"

    config.ssh.private_key_path = [ '~/.vagrant.d/insecure_private_key', '~/.ssh/id_rsa' ]
    config.ssh.forward_agent = true

end
