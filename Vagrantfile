# -*- mode: ruby -*-
# vi: set ft=ruby :


Vagrant.configure(2) do |config|
  config.ssh.insert_key = false

  config.vm.define "vagrant1" do |vagrant1|
    vagrant1.vm.box = "hashicorp/precise32"
    vagrant1.vm.network "forwarded_port", guest: 80, host: 8080
    vagrant1.vm.network "forwarded_port", guest: 443, host: 8443
    vagrant1.vm.provider "virtualbox" do |vb|
      vb.memory = "512"
    end
  end

config.vm.define "vagrant2" do |vagrant2|
    vagrant2.vm.box = "hashicorp/precise32"
    vagrant2.vm.network "forwarded_port", guest: 80, host: 8081
    vagrant2.vm.network "forwarded_port", guest: 443, host: 8444
    vagrant2.vm.provider "virtualbox" do |vb|
      vb.memory = "512"
    end
  end

config.vm.define "vagrant3" do |vagrant3|
    vagrant3.vm.box = "hashicorp/precise32"
    vagrant3.vm.network "forwarded_port", guest: 80, host: 8082
    vagrant3.vm.network "forwarded_port", guest: 443, host: 8445
    vagrant3.vm.provider "virtualbox" do |vb|
      vb.memory = "512"
    end
  end

end
