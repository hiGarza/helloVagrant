Vagrant.configure("2") do |config|
	config.vm.box = "ubuntu/trusty64"

	config.vm.provider "virtualbox" do |vb|
		vb.name = "helloVagrant"
		vb.memory = "512"
	end

	config.vm.network "forwarded_port", guest: 80, host: 8080
	config.vm.network "public_network", type: "dhcp"

end