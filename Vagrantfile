Vagrant.configure("2") do |config|

  config.vm.box = "bento/ubuntu-16.04"

  config.vm.network :private_network, ip: "192.168.76.76"
  config.ssh.insert_key = false

  config.vm.provider :virtualbox do |v|
    v.memory = 512
  end
end
