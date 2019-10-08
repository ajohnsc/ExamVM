# Exam VM
======
This is a simple ExamVM using vagrant this is the needed resources:
| Resources | Size |
| --- | --- |
| vCPU | 1 |
| Ram | 1024MB |
| Disk | 100GB |

Also you need to install the following:

1. VirtualBox click the link [here](https://www.virtualbox.org/wiki/Downloads)
1. Vagrant click the link [here](https://www.vagrantup.com/downloads.html)

======
## Setup the VM

1. add the vagrant box in your box list
`vagrant box add ajscanlas/examvm`

1. Initialize vagrant file
`vagrant init ajscanlas/examvm`

1. Start the VM
`vagrant up`

1. Connect to the examvm
`vagrant ssh`
======
## Tasks

1. Disable SELinux
> Disable SELinux and reboot the VM

1. Disable Firewall
> Disable Firewall permanently

1. Mount ISO as repository
> Inside the VM, there is a Centos iso, mount it as your local repository

1. Extend the partition
> 1. Extend the home partition to 20GiB in the LVG
> 2. Extend the root partition to 20GiB in the LVG

1. Install services needed
> 1. Install the HTTPD
> > 1. Change the port from 80 to 8080
> > 2. Add /home/vagrant/index.html file in the default web server directory
> > 3. Make sure that it is started automatically after reboot
> 2. Install MariaDB
> > 1. Change the port from port 3306 to 6033
> > 2. Make sure that it is started automatically after reboot

1. Run exam checker
> run `exam-check` command for the results
