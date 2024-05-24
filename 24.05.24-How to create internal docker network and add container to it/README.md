# How to create internal docker network and add container to it

```
docker run --name my_nginx_1 -itd -p 8081:80 nginx  
docker run --name my_nginx_2 -itd -p 8082:80 nginx

docker network create --internal nginx-network  

docker network connect nginx-network my_nginx_1 
docker network connect nginx-network my_nginx_2

docker exec -it my_nginx_1 curl my_nginx_2  

# Disconnect and remove containers (for cleanup)
docker network disconnect nginx-network my_nginx_1
docker network disconnect nginx-network my_nginx_2

docker stop my_nginx_1 my_nginx_2
docker rm my_nginx_1 my_nginx_2

docker network rm nginx-network
```