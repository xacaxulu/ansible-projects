VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
    config.vm.box = "opscode-ubuntu-14.04"
    config.vm.box_url = "http://files.vagrantup.com/precise32.box"

    config.vm.network :public_network

    config.vm.provision "ansible" do |ansible|
        ansible.playbook = "playbook.yml"
    end
end
