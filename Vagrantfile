# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure('2') do |config|
  config.vm.box      = 'centos64'
  config.vm.hostname = 'rails-dev-box-centos'

  config.vm.network :forwarded_port, guest: 3000, host: 3000

  config.vm.synced_folder './', '/vagrant'

  config.vm.provision :shell, path: 'bootstrap.sh'
end
