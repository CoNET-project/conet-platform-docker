# CONET Platform local launch environment

This repository provides a docker-compose file to provide local server to launch CONET platform to use CONET WEB3 browser. Packaged [NodeJS](https://nodejs.org/en) and [CONET platfrom](https://github.com/CoNET-project/seguro-platform) 

This sets up a single local website to host the PWA of CONET platfrom.

## Using

First, install Docker. Then, run:

```
git clone https://github.com/rauljordan/eth-pos-devnet && cd eth-pos-devnet
./clean.sh
docker compose up -d
```

You will see the following:

```
$ docker compose up -d
[+] Running 7/7
 ✔ Network conet-docker_default                   Created 
 ✔ Container conet-docker-conet-platform-local-1  Started
```

Next, you can inspect the logs of the different services launched. 

```
docker logs conet-docker-conet-platform-local-1 -f
```

You can open CONET Platform by local server use URL

http://localhost:3001

# Available Features

