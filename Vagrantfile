# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "Microsoft/EdgeOnWindows10"
  config.vm.box_check_update = false

  config.ssh.insert_key = false
  config.vm.provider "virtualbox" do |vb|
    # Display the VirtualBox GUI when booting the machine
    vb.gui = true
  
    # Customize the amount of memory on the VM:
    vb.memory = "1024"
    vb.customize ["modifyvm", :id, "--vram", "256"]
    vb.customize ['modifyvm', :id, '--usb', 'on']

  end
end
