# Atsumeru

Atsumeru runs in docker and is used as a self-hosted book server. With it, I can orgainize, manage, and read novels
rather easily. I'm using the container from [atsumerudev/atsumeru](https://hub.docker.com/r/atsumerudev/atsumeru). 
The run command on that page was necessary to have it run on portainer. Sadly, Atsumeru has not been updatd 
since last year, so I may have to search for a different hosting service.

## Configuration

```
docker run -d \
    --name=atsumeru \
    -p 31337:31337 \
    -v /path/to/your/library:/home/remus/media \
    -v /path/to/your/config:/container/atsumeru \
    -v /path/to/your/db:/container/atsumeru \
    -v /path/to/your/cache:/container/atsumeru \
    -v /path/to/your/logs:/container/atsumeru \
    --restart unless-stopped \
    atsumerudev/atsumeru:latest
```