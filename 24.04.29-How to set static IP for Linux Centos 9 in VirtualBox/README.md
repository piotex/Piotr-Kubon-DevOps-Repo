# How to set static IP for Linux Centos 9 in VirtualBox

https://youtube.com/shorts/1WGglAr97VE?feature=share

```
How to set static IP for Linux Centos 9 in VirtualBox

First, we need to stop our machine

Click on settings

Network 

and add a network card

select the Host-only Adapter type

click ok 

and start the machine

on the host, run the `ifconfig` command and save the number of the new network adapter card

run the `nmtui` command and click Edit connection

add

enter Profile name and Device as on the screen

add address and gateway

click ok

BACK and OK

now we can check the IP address with the `ifconfig` command

we can also try to log in by ssh

And thats it
```