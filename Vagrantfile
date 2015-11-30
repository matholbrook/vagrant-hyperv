
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(2) do |config|
  config.vm.box = "base"
  config.vm.synced_folder "." , "/vagrant", :disabled => true
  config.vm.provider "hyperv" do |hv, override|
    override.ssh.username = "vagrant"
    override.ssh.private_key_path = "~/.ssh"
  end  # |hv, override|
end  # |config|
