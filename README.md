# Pintos

## Project 0

Welcome to 14-712 Operating System!

Your first warming-up project consists of following the instruction below, preparing a working development environment for your future projects, and reading some code of Pintos. 

There is no deliverable for this project. Please feel free to come to office hours if you need any help. 

You're free to use any other methods you like to build up a development environment. We will only examine the pintos\src directory for grading purpose in the future projects. 

## Prepare the development environment

1. Download and install VirtualBox from its [website](https://www.virtualbox.org/wiki/Downloads)

As we found from (https://github.com/hashicorp/vagrant/issues/11249), Vagrant seems to be not supporting VirtualBox with version number larger than 6.1.

Please download version 6.0 or use the workarounds mentioned in this [issue](https://github.com/oracle/vagrant-boxes/issues/178#issue-536720633)

Windows users please disable Hyper-V, otherwise the VirtualBox environment will not boot. 

2. Download and install vagrant from its [website](https://www.vagrantup.com/downloads.html).

You can also use whatever package management tool you like for the softwares above.

3. You may also need to install X-Server for displaying the QEMU or Bochs windows. 

4. Clone this repository

```
git clone https://github.com/YorkHe/pintos.git
```

Windows users, please change the EOL sequence of file `pintos\src\misc\bochs-2.6.2-build.sh` to LF. Otherwise the vagrant script will not work properly. 

5. Go to the root of the repository, then run `vagrant up`. This may take a while. Please do this with good Internet connection.

6. Run `vagrant ssh` to log into the VM. The source code will be placed under the path `/home/vagrant/pintos`, and it is synced with the `pintos` directory in this repository.

7. HAVE FUN!

## Read the Codes

For having a better start of the first project, please read the following files. 

1. All the data structures under `lib/kernel` -- the `list`, `bitmap` and `hash`. They will be your best friends throughout this semester.
2. `threads/thread.h`, for a good understanding of what are stored in each thread and how the scheduler works. 
3. `threads/switch.S`. Try to understand how context switch happens in Pintos. 
4. `threads/synch.h` and `threads/synch.c`. What are the synchronization methods used in Pintos, and what are the differences?