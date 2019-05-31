Vagrant.configure("2") do |config|

config.vm.define "web" do |web|
    web.vm.box = "web"
    web.vm.box = "centos/7"
     web.vm.network "private_network", ip: "192.168.33.10"
     config.vm.provision "ansible" do |ansible|
        ansible.playbook = "examples/playbook-3/playbook.yml"
     end
  end

  config.vm.define "db" do |db|
      db.vm.box = "db"
      db.vm.box = "ubuntu/xenial64"
       db.vm.network "private_network", ip: "192.168.33.20"
    end
     #config.vm.provision "ansible" do |ansible|
     #   ansible.playbook = "examples/playbook-4/playbook.yml"
     #end
end
