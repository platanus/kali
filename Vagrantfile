Vagrant.configure("2") do |config|
  config.vm.box = "https://storage.googleapis.com/pl-vagrant/virtualbox.box"
  
  config.ssh.private_key_path = 'ssh-keys/pentest-env'
  config.ssh.username = 'root'  
  
  config.vm.guest = :debian
  config.vm.provider "virtualbox" do |v|
    v.gui = true
    v.customize ['modifyvm', :id, '--memory', 2048]
  end
end


