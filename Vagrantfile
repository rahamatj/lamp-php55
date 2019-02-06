# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

    config.vm.box = "ubuntu/trusty64"

    config.vm.provider "virtualbox" do |v|
        v.memory = 512
        v.cpus = 1
    end

    config.vm.define :lamp_php55 do |lamp_config|
        lamp_config.vm.hostname = 'lamp-php55'
        lamp_config.vm.network "private_network", ip: "192.168.55.90"
        lamp_config.vm.provision :shell, path: "bootstrap.sh"
    end

    config.vm.provider :virtualbox do |vb_config|
        vb_config.name = "Vagrant - Ubuntu 14.04 LAMP - PHP 5.5"
    end

    config.vm.synced_folder "public", "/var/www/html"

end
