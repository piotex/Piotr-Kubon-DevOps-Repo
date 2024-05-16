# How to run basic Ansible playbook 

https://youtube.com/shorts/eO7sJsEzP-g?feature=share

```
vi inventory.yml
vi playbook.yml

ansible-playbook -i inventory.yml playbook.yml --private-key /home/peter/.ssh/id_rsa-ansible_user-192.168.56.62

sudo firewall-cmd --zone=public --add-port=80/tcp --permanent
sudo firewall-cmd --reload
```