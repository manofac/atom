# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
  config.vm.box = "bento/centos-7.6"
  config.vm.network "private_network", ip: "192.168.33.10"
  # OS -> VMの同期フォルダ紐付け
  config.vm.synced_folder "./", "/vagrant", :mount_options => ['dmode=777', 'fmode=777']
  config.vm.provision :shell, :path => "provision.sh"
end