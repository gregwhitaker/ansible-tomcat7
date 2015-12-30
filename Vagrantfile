Vagrant.configure(2) do |config|
    config.vm.box = "ubuntu/trusty64"
    config.vm.network "private_network", ip: "192.168.0.10"
    config.vm.hostname = "mytrusty.box"

    config.vm.provision "ansible" do |ansible|
    	ansible.playbook = "site.yml"
  	end
end 