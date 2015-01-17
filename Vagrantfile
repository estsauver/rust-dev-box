# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.provision "shell", inline: "apt-get --assume-yes install g++"
  config.vm.provision "shell", inline: "apt-get --assume-yes install python"
  config.vm.provision "shell", inline: "apt-get --assume-yes install perl"
  config.vm.provision "shell", inline: "apt-get --assume-yes install make"
  config.vm.provision "shell", inline: "apt-get --assume-yes install curl"
  config.vm.provision "shell", inline: "apt-get --assume-yes install git"
  config.vm.provision "shell", inline: "mkdir /home/vagrant/dev"
  config.vm.provision "shell", inline: "cd /home/vagrant/dev/ && git clone https://github.com/rust-lang/rust.git"
  config.vm.provision "shell", inline: "cd /home/vagrant/dev/rust/ && ./configure"
  config.vm.provision "shell", inline: "cd /home/vagrant/dev/rust/ && chmod -R 777 . && make && make install"

  # Provider specific settings.
  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
    v.cpus = 2
  end
end
