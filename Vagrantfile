# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  # All Vagrant configuration is done here. The most common configuration
  # options are documented and commented below. For a complete reference,
  # please see the online documentation at vagrantup.com.

  # Every Vagrant virtual environment requires a box to build off of.
  config.vm.box = "centos5.8"

  # The url from where the 'config.vm.box' box will be fetched if it
  # doesn't already exist on the user's system.
  config.vm.box_url = "http://tag1consulting.com/files/centos-5.8-x86-64-minimal.box"

  Vagrant::Config.run do |config|
    config.vm.provision :shell, :inline => "bash /vagrant/INSTALL.txt; sudo cp /ff_sources/ffmpeg-1.2.1/ffprobe /vagrant/ffprobe-1-2-1-linux; sudo cp /ff_sources/ffmpeg-1.2.1/ffmpeg /vagrant/ffmpeg-1-2-1-linux"
  end



end
