# -*- mode: ruby -*-
# vi: set ft=ruby :


# Backwards compatibility
Vagrant.configure("2") do |config|
  config.vm.box = "base"

  # Expose port 80 as 8080 on the host machine
  config.vm.network "forwarded_port", guest: 80, host: 8080

  # VM config
   config.vm.provider "virtualbox" do |vb|
     # Disable the GUI
     vb.gui = false
  
     # Customize the amount of memory on the VM:
     vb.memory = "512"
   end
end
