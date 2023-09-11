# simple_Apache_web_server

A **Vagrantfile** was creadted using the `Vagrant up bento/ubuntu-16.04` command. It is a Ruby script that defines the configuration of a virtual machine using Vagrant . 

The purpose of this code is to create and configure a virtual machine that runs Ubuntu 16.04 with Apache2 installed. The virtual machine is named "osho" and has 1024 MB of memory allocated to it. The `synced_folder` directive maps the `./html` directory on the host machine to the `/var/www/html` directory on the guest machine . This allows the sharing of files between the host and guest machines.

The `provision` directive installs Apache2 on the guest machine using a shell script . The `run: "always"` option ensures that the script is run every time the virtual machine is started .

This set-up was created to run as a single virtual machine on top of windows 11 host machine.

With the help of vagrant, the enviroment was configure, so that it will run an Apache web server on port `80` of the virtual machine and the port will be mapped to the port `8080` of the host machine.
