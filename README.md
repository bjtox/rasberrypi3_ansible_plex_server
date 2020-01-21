# raspberrypi3_ansible_plex_server
A playbook to install plexServer on debian based OS

UNDER COSTRUCTION

## Requirements
* raspberrypi 2/3
* installed distro based on debian
* a service user like "ansible" with a private key on Remote HOST

## HOW to use

This playbook made a simple installation of plex media plexServer.
After installation you can open a web interface of PLEX on `http://<hostname>:32400/web/`

###### Required Vars
```yml
---
remote_user: pi
plex_custom_remote_user: "{{ remote_user }}"
```
###### Run
```bash
ansible-playbook plays/install_plex.yml
```


#### Credits
Playbook based on [PiMyLifeUp installation guide](https://pimylifeup.com/raspberry-pi-plex-server/)

#### References
* https://www.raspberrypi.org/documentation/remote-access/ssh/passwordless.md


###### Tags
- raspberrypi
- raspbian
- debian
- ubuntu
- plexmediaserver
- plex
- ansible
