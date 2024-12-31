# Main Server // HP EliteDesk 

This small server is perfect for a small sized homelab and can be upgraded in the future if necessary. They provide 
enough computing power for most tasks and combined have 16GB of RAM. This server was the first of
my actual hardware I bought.

## Specifications

| CPU            | RAM | Storage  | OS                  | Hostname | IP (/24)	  |
| -------------- | --- | -------- | ------------------  | -------- | -----------  |
| Intel i5-6500T | 4GB | 39GB SSD | Proxmox (baremetal) | soup     | 192.168.1.17 |
| Intel i5-6500T | 4GB | 32GB SSD | Debian 12           | pork     | 192.168.1.14 |
| Intel i5-6500T | 4GB | 20GB SSD | Ubuntu LXC          | calzone  | 192.168.1.18 |

## Services

This server currently runs most of my services that I self-host. You can find out more about the services running 
in this cluster [here](/services/service-lists/). 

### Converting from Windows to New OS

1. Create a bootable USB with desired operating system
2. When booting up, press F12
3. Allow "boot from USB" in BIOS
4. Follow installer instructions

## Images

![EliteDesk](/images/hpelitedesk.jpg)
![EliteDesk](/images/Elite_Bot.JPG) 

