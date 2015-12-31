Vagrant.configure(2) do |config|
    config.vm.box = "ubuntu/trusty64"
    config.vm.network "private_network", ip: "192.168.0.10"
    config.vm.hostname = "mytrusty.box"
    config.vm.provider "virtualbox" do |v|
    	v.name = "ansible-tomcat7"
    	v.memory = 2048
    end

    config.vm.provision "ansible" do |ansible|
    	ansible.playbook = "site.yml"
  	end
end 