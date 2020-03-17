Virtual Box and Vagrant

Vagrant init - starts up a vagrant file that allows you to create virtual machine
Vagrantile
```ruby
Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/bionic64" # operating system
  config.vm.network "private_network", ip: "192.168.10.100" # connection to server


end
```
`Vagrant up` - creates the virtual machine
`Vagrant destroy` - destroys the virtual machine
`Vagrant ssh` - enters the virtual machine
`Vagrant reload` - reboots the VM


Inside the virtual machine

Sudo - allows you to perform root commands
Apt - package manager, same as pip for python
-y - ignores the are you sure check
`ps aux | grep` - checks if something is running
`sudo systemctl start` - starts a package you install

`exit` - leaves the virtual machine
