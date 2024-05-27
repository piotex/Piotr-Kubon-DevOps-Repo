# Linux-What are the basic docker commands

https://youtube.com/shorts/ErOBZlVgnPU?si=yensXT4byo4Vizgj

```
docker run hello-world
docker ps
docker ps -a
docker run -itd nginx
docker run --name my_nginx -itd -p 8080:80 nginx
docker exec -it mycontainer /bin/bash     or   sh
docker stop mycontainer 
docker rm mycontainer 
docker run --name my_nginx -itd -p 8080:80 nginx
docker exec -it 09 curl localhost
docker images
```