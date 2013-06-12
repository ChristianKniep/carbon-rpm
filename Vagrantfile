Vagrant.configure("2") do |config|
  config.vm.box = "centos64-dev"
  config.vm.synced_folder "../.", "/git"
  config.vm.provider "virtualbox" do |v|
    v.customize ["modifyvm", :id, "--cpuexecutioncap", "75"]
  end
end

