# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"

  config.vm.provision "shell" do |s|
    s.privileged = false
    s.inline = <<-SHELL
      curl -fsSL https://get.pulumi.com | sh

      curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
      sudo apt-get install -y nodejs
    SHELL
  end

end
