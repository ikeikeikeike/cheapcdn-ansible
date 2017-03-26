# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  # All Vagrant configuration is done here. The most common configuration
  # options are documented and commented below. For a complete reference,
  # please see the online documentation at vagrantup.com.

  # Every Vagrant virtual environment requires a box to build off of.
  config.vm.box = "ubuntu/xenial64"

  config.vm.provider "virtualbox" do |provider|
    # Don't boot with headless mode
    # vb.gui = true

    # Use VBoxManage to customize the VM. For example to change memory:
    provider.customize [
      "modifyvm", :id,
      "--memory", "512",
      # "--cpus", "1",
      # "--ioapic", "on"
    ]
  end

  config.vm.define :"object1" do |web|
    web.vm.provider :virtualbox do |vbox|
      vbox.name = "object1"
    end

    # web.vm.network :forwarded_port, host: 8001, guest: 8000
    web.vm.network :private_network, ip: "192.168.33.25"
    web.vm.network "public_network", ip: "192.168.10.100"
    web.vm.network :forwarded_port, host: 8005, guest: 8000
    web.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2225
  end

  config.vm.define :"object2" do |web|
    web.vm.provider :virtualbox do |vbox|
      vbox.name = "object2"
    end

    # web.vm.network :forwarded_port, host: 8001, guest: 8000
    web.vm.network :private_network, ip: "192.168.33.26"
    web.vm.network "public_network", ip: "192.168.10.101"
    web.vm.network :forwarded_port, host: 8006, guest: 8000
    web.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2226
  end

  config.vm.define :"object3" do |web|
    web.vm.provider :virtualbox do |vbox|
      vbox.name = "object3"
    end

    # web.vm.network :forwarded_port, host: 8001, guest: 8000
    web.vm.network :private_network, ip: "192.168.33.27"
    web.vm.network "public_network", ip: "192.168.10.102"
    web.vm.network :forwarded_port, host: 8007, guest: 8000
    web.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2227
  end

  config.vm.define :"object4" do |web|
    web.vm.provider :virtualbox do |vbox|
      vbox.name = "object4"
    end

    # web.vm.network :forwarded_port, host: 8001, guest: 8000
    web.vm.network :private_network, ip: "192.168.33.28"
    web.vm.network "public_network", ip: "192.168.10.103"
    web.vm.network :forwarded_port, host: 8008, guest: 8000
    web.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2228
  end

  config.vm.define :"object5" do |web|
    web.vm.provider :virtualbox do |vbox|
      vbox.name = "object5"
    end

    # web.vm.network :forwarded_port, host: 8001, guest: 8000
    web.vm.network :private_network, ip: "192.168.33.29"
    web.vm.network "public_network", ip: "192.168.10.104"
    web.vm.network :forwarded_port, host: 8009, guest: 8000
    web.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2229
  end

  config.vm.define :"object6" do |web|
    web.vm.provider :virtualbox do |vbox|
      vbox.name = "object6"
    end

    # web.vm.network :forwarded_port, host: 8001, guest: 8000
    web.vm.network :private_network, ip: "192.168.33.30"
    web.vm.network "public_network", ip: "192.168.10.105"
    web.vm.network :forwarded_port, host: 8010, guest: 8000
    web.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2230
  end

  # config.vm.define :"object7" do |web|
  #   web.vm.provider :virtualbox do |vbox|
  #     vbox.name = "object7"
  #   end

  #   # web.vm.network :forwarded_port, host: 8001, guest: 8000
  #   web.vm.network :private_network, ip: "192.168.33.31"
  #   web.vm.network "public_network", ip: "192.168.10.106"
  #   web.vm.network :forwarded_port, host: 8011, guest: 8000
  #   web.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2231
  # end

  # config.vm.define :"object8" do |web|
  #   web.vm.provider :virtualbox do |vbox|
  #     vbox.name = "object8"
  #   end

  #   # web.vm.network :forwarded_port, host: 8001, guest: 8000
  #   web.vm.network :private_network, ip: "192.168.33.32"
  #   web.vm.network "public_network", ip: "192.168.10.107"
  #   web.vm.network :forwarded_port, host: 8011, guest: 8000
  #   web.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2232
  # end


end
