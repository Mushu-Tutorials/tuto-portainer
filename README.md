# tuto-portainer

Here the `docker-compose.yml` to run the portainer container:

```yml
version: '3'
services:
  portainer-ce:
    image: portainer/portainer-ce
    container_name: "portainer"
    ports: 
      - "9000:9000"
    volumes: 
      - /var/run/docker.sock:/var/run/docker.sock
```