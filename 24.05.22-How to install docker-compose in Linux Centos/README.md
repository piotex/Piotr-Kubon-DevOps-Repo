# How to install docker-compose in Linux Centos 

https://youtube.com/shorts/hUypqYwFkKY
https://youtube.com/shorts/hUypqYwFkKY?feature=share
https://youtube.com/shorts/hUypqYwFkKY?si=GsWTXBleusQu_oP5

```
 sudo yum update -y
 sudo yum install docker-compose-plugin -y
 docker compose version
 ```
 ```
 vi docker-compose-file.yml
```
```
services:
    client:
        image: nginx
        ports:
            - 8080:80
```
```
docker compose -f docker-compose-file.yml build
docker compose -f docker-compose-file.yml up -d
docker ps -a
```
```
sudo firewall-cmd --zone=public --add-port=8080/tcp --permanent
sudo firewall-cmd --reload
```