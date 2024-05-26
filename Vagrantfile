Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"

  # Shared folder configuration
  config.vm.synced_folder ".", "/vagrant", type: "virtualbox"

  # Port forwarding
  config.vm.network "forwarded_port", guest: 12344, host: 12344

  # Provisioning the VM with shell script
  config.vm.provision "shell", inline: <<-SHELL
    # Update package list
    sudo apt-get update
    
    # Install the hello_http package
    sudo apt-get install -y build-essential

    # Additional setup commands if needed
    # ...
  SHELL
end
