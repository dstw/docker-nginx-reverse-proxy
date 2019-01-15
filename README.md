# Nginx Reverse Proxy

## Summary

The purpose of this docker is to give an example of Nginx application to
perform reverse proxy on containers. In short words, it can map different container using
HTTP port to use different Domain Name in the same IP address.  
This is based on https://www.thepolyglotdeveloper.com/2017/03/nginx-reverse-proxy-containerized-docker-applications.

## Prerequisite

Docker (of course!)

## Usage

	$ git clone https://github.com/dstw/docker-nginx-reverse-proxy
	$ docker-compose up -d

Add to your /etc/hosts:

	docker-host-ip      docker-nginx
	docker-host-ip      docker-apache
	docker-host-ip      docker-lighttpd
	docker-host-ip      srv1
	docker-host-ip      srv2
	docker-host-ip      srv3

Then you can see different page on that names.
