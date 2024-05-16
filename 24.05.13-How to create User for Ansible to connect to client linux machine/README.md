# How to create User for Ansible to connect to client linux machine

https://youtube.com/shorts/c-VxmKw6I78?feature=share

On Client
```
sudo useradd ansible_user
sudo passwd ansible_user

sudo visudo
    ansible_user ALL=(ALL) NOPASSWD:ALL
```

On Main
```
ssh-keygen -t rsa -b 2048 -C "ansible_user@192.168.56.62"
    /home/peter/.ssh/id_rsa-ansible_user-192.168.56.62

ssh-copy-id -i /home/peter/.ssh/id_rsa-ansible_user-192.168.56.62   ansible_user@192.168.56.62

ssh -i /home/peter/.ssh/id_rsa-ansible_user-192.168.56.62     ansible_user@192.168.56.62
```