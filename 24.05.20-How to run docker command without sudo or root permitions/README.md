# How to run docker command without sudo or root permitions

```
sudo groupadd docker
sudo usermod -aG docker $USER
newgrp docker
docker run hello-world
```