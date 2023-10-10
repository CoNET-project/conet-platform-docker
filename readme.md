# CONET Platform local launch environment

This repository provides a docker-compose file to provide local server to launch CONET platform to use CONET WEB3 browser. Packaged [NodeJS](https://nodejs.org/en) and [CONET platfrom](https://github.com/CoNET-project/seguro-platform) 

This sets up a single local website to host the PWA of CONET platfrom.

This docker image packaged CONET software include 

@conet-project/conet-platform 0.60.3
@conet.project/seguro-gateway 0.18.6


## Using

First, install Docker. Then, run:

```
git clone https://github.com/CoNET-project/conet-platform-docker && cd conet-platform-docker
docker-compose up -d
```
You will see the following:

```
$ docker-compose up -d
[+] Running 7/7
 ✔ Network conet-docker_default                   Created 
 ✔ Container conet-docker-conet-platform-local-1  Started
```

Next, you can inspect the logs of the different services launched. 

```
docker logs conet-platform-docker-conet-platform-local-1 -f
```

Open CONET Platform by local server use URL to unlock wallet

http://localhost:3001


### Stop Docker

$ docker stop conet-platform-docker-conet-platform-local-1

```
docker stop conet-platform-docker-conet-platform-local-1
```

## Available Features

Use Proxy

Only for Sock v5 support Proxy DNS

proxy server localhost
proxy port 3002