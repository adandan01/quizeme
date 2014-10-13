# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.box = "trusty64"
    config.vm.box_url = "https://vagrantcloud.com/ubuntu/trusty64/version/1/provider/virtualbox.box"

    config.vm.network :forwarded_port, guest: 9000, host: 9000

    # # Add to /etc/hosts: 33.33.33.24 dev.example.com
    # config.vm.network :hostonly, "33.33.33.24"

    # provision with simple shell script
    config.vm.provision "shell", path: "install_requirements.sh"
end
