Vagrant.configure('2') do |config|
	config.vm.provider :digital_ocean do |provider, override|
		override.ssh.private_key_path = '~/.ssh/id_rsa'
		provider.ssh_key_name = '<sample ssh key name>'
		override.vm.box = 'digital_ocean'
		override.vm.box_url = "https://github.com/smdahlen/vagrant-digitalocean/raw/master/box/digital_ocean.box"

        provider.token = '<DO token>'
		provider.image = 'ubuntu-14-04-x64'
		provider.region = 'nyc3'
		provider.size = '512mb'
	end
	config.vm.provision "ansible" do |ansible|
		ansible.playbook = "playbook.yml"
	end
end
