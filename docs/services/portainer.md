# Portainer

Portainer is a web-GUI that is helpful for managing/deploying/editing docker containers. As I get more
understanding with docker compose, I may transition from portainer to that.

## Setup 

Setup:

First created a LXC container using Ubuntu as the template
	Installed Docker using apt repository https://docs.docker.com/engine/install/ubuntu/
	Install Portainer for a GUI
			See Configuration below
	Install net tools 
			 apt install net-tools

To enter Portainer, enter Calzone IP with Portainer’s port (9443) in search bar

### Configuration

The docker run command 

```
docker run -d \
	-p 8000:8000 \
	-p 9443:9443 \
	--name portainer \
	--restart=always \
	-v /var/run/docker.sock:/var/run/docker.sock \
	-v portainer_data:/data \
	portainer/portainer-ce:latest
```