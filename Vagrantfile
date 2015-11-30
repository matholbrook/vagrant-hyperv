
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(2) do |config|
  config.vm.box = "base"
  config.vm.box.url = "https://atlas.hashicorp.com/hashicorp/boxes/precise64
  config.vm.synced_folder "." , "/vagrant", :disabled => true
  config.vm.provider "hyperv" do |hv, override|
    hv.vmname = "CLD-HV-MH1"
    hv.cpus   = 1
    hv.memory = 512
    override.ssh.username = "vagrant"
    override.ssh.private_key_path = "~/.ssh"
  end  # |hv, override|
end  # |config|
