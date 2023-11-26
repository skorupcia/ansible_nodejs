# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  # General Vagrant VM configuration.
  config.vm.box = "luminositylabsllc/bento-rockylinux-9-aarch64"
  config.ssh.insert_key = false
  config.vm.synced_folder ".", "/vagrant", type: "rsync",
    rsync__exclude: ".git/"
  config.vm.provider "parallels" do |prl|
    prl.memory = 512
    prl.linked_clone = true
  end
  # Application server.
  config.vm.define "nodejs" do |app|
    app.vm.hostname = "nodejs.test"
    app.vm.network :private_network, ip: "192.168.56.9"
  end
end
