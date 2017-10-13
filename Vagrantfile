# -*- mode: ruby -*-

Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/xenial64"

  config.vm.provision :ansible_local do |ansible|
    ansible.install = true
    ansible.playbook = "playbook.yml"
#  config.vm.provision :shell, path: "bootstrap.sh" ## Placeholder for the time I would need Bootstrap
  end
   config.vm.network "forwarded_port", guest: 80, host: 5005

end
