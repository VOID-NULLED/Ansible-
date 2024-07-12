Vagrant.configure("2") do |config|

  config.vm.define "nginx" do |nginx|
    nginx.vm.box = "ubuntu/bionic64"
    nginx.vm.network "private_network", ip: "192.168.33.10"
    nginx.vm.hostname = "nginx"
    nginx.vm.provider "virtualbox" do |vb|
      vb.memory = "512"
    end
  end

  config.vm.define "apache" do |apache|
    apache.vm.box = "ubuntu/bionic64"
    apache.vm.network "private_network", ip: "192.168.33.11"
    apache.vm.hostname = "apache"
    apache.vm.provider "virtualbox" do |vb|
      vb.memory = "512"
    end
  end

end
