## Requirements

- virtualbox
- iso for redhat or centos
- virtual network editor
- we need virtual network editor to check NAT network and check ips to know them as we will use them later

## Installing our system

- open virtual network editor to get Nat subnet ip range you will find that after installing vmware
- open vm ware and select new virtual machine
- check custom vm
- name the vm machine and set location
- set 1 processor and 2 core processors
- for network use nat
- for I/O use recommended LSI Logic
- use recommended virtual disk type SCSI
- create virtual hard disk for 100 GB as a single file by changing the option (good option to take this file and use it in case of corrupted vm box)
- after creating the virtual machine you can change processor settings and select to create virtual machine inside of a virtual machine by selecting `virtualbox intel ot AMD` option
- connect network to set date and time
- disable KDUMP stands for kernal dump that take a dump from the kernal in case some errors and you contact the technical support they will ask for the kernal dump file to be sent to them for troubleshooting.
- software select , select `server with GUI`
- in installation destination select `configure partationing manually reset , rescan and select lvm type and choose automatically partation then done`.
- disable security
- create admin user and password
- then start installation and after finishing installation , reboot your system and login to remotely control the system
- now, run `ifconfig` and get the vm id `192.168.92.131`
- go to your machine open the terminal and `ssh imohamed@192.168.92.131` and enter the password of imohamed and then you can access the vm machine remotely
- on windows you can use a terminal emulator like `mobaxterm` that allows you to open many sessions
- in linux I use `xterminal` emulator
