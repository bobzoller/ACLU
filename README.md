# Code for Hawaii / ACLU Access to public lands in Hawai`i App
We're just getting started, stay tuned!

For now, please help fill out the [project board](https://github.com/CodeforHawaii/ACLU/projects/1).

## Development / Getting Started
To provide a consistent development setup, we've made scripts to provision a Linux virtual machine that runs Docker containers. _"yo :dog:..."_

If you don't know what that means, read the sections below. :arrow_down:

If you do, just make sure you have `VirtualBox` (v5.0+) and `vagrant` (v 1.9+), then run `vagrant up`. :clap:

### VirtualBox
[VirtualBox](https://www.virtualbox.org) is a product from [Oracle](https://www.oracle.com) that runs an entire Operating System (the _"guest OS"_) inside the VirtualBox program on your computer (the _"host OS"_).

:question: _Why on :earth_americas: would you want that?_  
 **A:** This allows us to encapsulate the entire development environment in the _guest OS_ without having to modify your _host OS_. Thus, we can install all the development tools we need without worrying about potentially breaking any configuration on your computer. It also gives us a common OS (Linux) that we know things will work on. :smiley:

Please [download VirtualBox here](https://www.virtualbox.org/wiki/Downloads) for your _host OS_ and install it.

### Vagrant
[Vagrant](https://www.vagrantup.com) is a [HashiCorp](https://www.hashicorp.com) product that provides a convenient scripting interface to control VirtualBox and manage Virtual Machines.

:question: _Again, why do you need this?_  
 **A:** Vagrant allows us to automatically configure the _guest OS/VM_ exactly how we want it in a consistent fashion. This means you won't have to spend time downloading, installing, and configuring the correct versions of development tools (e.g. node, yarn, python, httpie, docker, etc..) to setup your build environment.

Please [download Vagrant here](https://www.vagrantup.com/downloads.html) for your OS and install it.

### Creating the VM
After VirtualBox and Vagrant are installed, run the following command from the root directory of the `aclu` repo:
```
vagrant up
````
...and maybe grab some :coffee: and :doughnut: -- depending on your internet connection, this may take awhile!

### Running a shell in the VM
```
vagrant ssh
```
