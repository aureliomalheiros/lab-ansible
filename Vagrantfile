Vagrant.configure("2") do |config|
	
	config.vm.define "webserver" do |webserver|
			webserver.vm.box = "ubuntu/xenial64"
			webserver.vm.network "private_network", ip:"10.10.10.11"
			webserver.vm.hostname = "webserver"
			webserver.vm.provider "virtualbox" do |vb|
				vb.name = "webserver"
			end
			webserver.vm.provision "shell", inline: <<-SHELL
			SHELL
	end
	config.vm.define "database" do |database|
		database.vm.box = "centos/7"
		database.vm.network "private_network", ip: "10.10.10.12"
		database.vm.hostname = "database"
		database.vm.provider "virtualbox" do |vb|
			vb.name = "database"
		end
		database.vm.provision "shell", inline: <<-SHELL
		SHELL
	end
end
