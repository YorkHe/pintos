# Pintos

## Prepare the development environment

1. Download and install VirtualBox from its [website](https://www.virtualbox.org/wiki/Downloads)

As we found from (https://github.com/hashicorp/vagrant/issues/11249), Vagrant seems to be not supporting VirtualBox with version number larger than 6.1.

Please download version 6.0 or use the workarounds mentioned in this [issue](https://github.com/oracle/vagrant-boxes/issues/178#issue-536720633)

2. Download and install vagrant from its [website](https://www.vagrantup.com/downloads.html).

You can also use whatever package management tool you like for the two softwares above.

3. Clone this repository

```
git clone https://github.com/YorkHe/pintos.git
```

4. Go to the root of the repository, then run `vagrant up`. This may take a while. Please do this with good Internet connection.

5. Run `vagrant ssh` to log into the VM. The source code will be placed under the path `/home/vagrant/pintos`, and it is synced with the `pintos` directory in this repository.

6. HAVE FUN!
