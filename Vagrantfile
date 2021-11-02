Vagrant.configure("2") do |config|
  config.vm.box = "debian/bullseye64"

  config.vm.provision "ansible", run: "always" do |ansible|
    ansible.playbook = "init.yaml"
    ansible.galaxy_role_file = "requirements.yaml"
  end
end
