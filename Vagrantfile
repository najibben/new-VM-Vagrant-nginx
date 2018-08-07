Vagrant.configure("2") do |config|
config.vm.box = "hashicorp/precise64"
config.vm.hostname = "devopsweb01.vagrant.vm"
#config.vm.provision "shell", path: "provision.sh"
config.vm.provision :shell, :path => ".provision/bootstrap.sh"
config.vm.network :private_network, ip: "192.168.30.30"
config.vm.network "forwarded_port", guest: 80, host: 8081, id: "nginx"
end
