Vagrant.configure("2") do |config|
  # Gunakan box Ubuntu 20.04
  config.vm.box = "ubuntu/focal64"

  # Server 1 (Galera node 1)
  config.vm.define "node1" do |node1|
    node1.vm.hostname = "node1"
    node1.vm.network "private_network", ip: "192.168.56.11"
    node1.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end

  # Server 2 (Galera node 2)
  config.vm.define "node2" do |node2|
    node2.vm.hostname = "node2"
    node2.vm.network "private_network", ip: "192.168.56.12"
    node2.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end

  # Server 3 (Galera node 3)
  config.vm.define "node3" do |node3|
    node3.vm.hostname = "node3"
    node3.vm.network "private_network", ip: "192.168.56.13"
    node3.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end

  # Server 4 (MaxScale)
  config.vm.define "maxscale" do |maxscale|
    maxscale.vm.hostname = "maxscale"
    maxscale.vm.network "private_network", ip: "192.168.56.14"
    maxscale.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end
  end
end