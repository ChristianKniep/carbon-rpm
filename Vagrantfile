Vagrant.configure("2") do |config|
  config.vm.box = "centos64-dev20130612.1"
  config.vm.network :forwarded_port, guest: 80, host: 8080
  config.vm.synced_folder "../.", "/git"
  config.vm.provider "virtualbox" do |v|
    v.customize ["modifyvm", :id, "--cpuexecutioncap", "75"]
  end
end

