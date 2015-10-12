Vagrant.configure(2) do |config|
  config.vm.box = "centos7"
  config.vm.network "private_network", ip: "192.168.33.10"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible/site.yaml"
    ansible.inventory_path = "ansible/hosts"
    ansible.limit = 'all'
  end
end
