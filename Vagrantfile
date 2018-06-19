Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/xenial64"

  config.vm.network "private_network", ip: "192.168.33.20"

  config.vm.provider "virtualbox" do |vb|
     vb.name = "mbtiles-generator"
     vb.memory = "4096"
  end

  config.vm.provision "provision-docker", type: "shell" do |s|
    s.path = "provision/provision-docker.sh"
  end

end
