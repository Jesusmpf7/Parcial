Vagrant.configure("2") do |config|
    # Configuración común para todas las máquinas
    config.vm.box = "ubuntu/bionic64"
    config.vm.network "private_network", type: "dhcp"
  
    # Configuración para la primera máquina
    config.vm.define "server1" do |server|
      server.vm.hostname = "server1"
      server.vm.network "forwarded_port", guest: 22, host: 2222
      server.vm.provider "virtualbox" do |vb|
        vb.memory = "256"
        vb.cpus = 1
      end
    end
  
    # Configuración para la segunda máquina
    config.vm.define "server2" do |server|
      server.vm.hostname = "server2"
      server.vm.network "forwarded_port", guest: 22, host: 2223
      server.vm.provider "virtualbox" do |vb|
        vb.memory = "256"
        vb.cpus = 1
      end
    end
  
    # Configuración para la tercera máquina
    config.vm.define "server3" do |server|
      server.vm.hostname = "server3"
      server.vm.network "forwarded_port", guest: 22, host: 2224
      server.vm.provider "virtualbox" do |vb|
        vb.memory = "256"
        vb.cpus = 1
      end
    end
  end
  