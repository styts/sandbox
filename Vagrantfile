VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.box_check_update = false
  config.vm.hostname = "sandbox"
  config.ssh.forward_agent = true
  config.vm.synced_folder "~/Dropbox/Projects", "/home/vagrant/Projects"

  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--memory", "4096"]
  end
end
