# How to run docker command without sudo or root permitions

https://youtube.com/shorts/CPYsmykLqVk?feature=share

```
sudo groupadd docker
sudo usermod -aG docker $USER
newgrp docker
docker run hello-world
```