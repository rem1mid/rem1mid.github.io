# Overview

This section will list all the services I run inside my homelab, how they are implemented (configs, notes, etc) and
links to documentation on the service.

In theory, I should be able to recreate my entire service stack from these docs alone.

## List of Services

- Factorio Server
- Plex
- Atsumeru
- Portainer
- Docat

## Service Topology

![Service Topology](https://i.dbyte.xyz/firefox_Rpz0o5ONP.png)


## Connecting to my HomeLab

I have set up my network and DNS in such a way to allow me to SSH to my HomeLab from anywhere in the world, except for China.
To do this, I used [Cloudflare](https://cloudflare.com) to allow me to dynamically update my DNS entries, as my home IP
is not static. Then I set up my domains to proxy through Cloudflare to hide my IP. Now you may be wondering how I connect
home if my IP is hidden from the world. The answer is disabling Cloudflare proxy on a subdomain. This allows my IP to
exposed through a domain name dynamically.
