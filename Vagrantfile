# -*- mode: ruby -*-

Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/trusty64"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  config.vm.provision :shell, path: "bootstrap.sh" ## Placeholder for the time I would need Bootstrap
  end
   config.vm.network "forwarded_port", guest: 80, host: 5005
   config.vm.network "forwarded_port", guest: 3306, host: 5006

end
