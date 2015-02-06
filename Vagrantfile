Vagrant.configure("2") do |config|
    config.vm.provider :virtualbox do |v|
        v.name = "web_scraper"
        v.customize ["modifyvm", :id, "--memory", 512]
    end

    config.vm.box = "trusty64"
    config.vm.box_url = "https://vagrantcloud.com/ubuntu/trusty64/version/1/provider/virtualbox.box"

    config.vm.network :private_network, ip: "192.168.10.100"
    config.ssh.forward_agent = true

end
