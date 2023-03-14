# Cours Docker ENSG
blabla

* Automation of DNS and Hosts naming + SSL certificates using [docker-gen](https://github.com/nginx-proxy/docker-gen) templates
* [mkcert](https://github.com/FiloSottile/mkcert) certificates + CA preconfigured for Mozilla Firefox Web browser
* [dnsmasq](https://thekelleys.org.uk/dnsmasq/doc.html) working server (port 53) and on-demand (`make set-hosts`) system `/etc/hosts` file with the following pattern : 
  * For every container exposing ports : `docker-compose.service`.`docker-compose.project`.docker record
  * For proxied services only : entries matching `VIRTUAL_HOST` resolve the nginx-proxy IP address
* Management of all your stacks and containers using [Portainer CE](https://hub.docker.com/r/portainer/portainer-ce)


**Table Of Contents:**
  - [Docker environment preparation](#docker-environment-preparation)

----

## Docker environment preparation 