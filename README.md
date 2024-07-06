# ![](https://github.com/CTFd/CTFd/blob/master/CTFd/themes/core/static/img/logo.png?raw=true)

# CTFd 3.5.0 with Docker Plugin for What's Your ETH CTF
This repository contains a modified version of CTFd 3.5.0 integrated with the Docker plugin, used to host the WhatyourETH CTF competition.

## Features
- CTFd 3.5.0 core functionality
- Docker plugin for efficient challenge deployment and management

## Usage
We use the Docker outside Docker (DooD) approach in this setup. This method allows the CTFd container to interact with the host's Docker daemon, providing better resource management.

You can build image and use images with the following command:

`docker build -t ctfd .`

`docker run -d -p 80:8000 -v /var/run/docker.sock:/var/run/docker.sock --group-add [docker_group_id] ctfd`

Or you can use Docker Compose with the following command from the source repository:

`docker compose build --no-cache`

`docker compose up`

Note: The `-v /var/run/docker.sock:/var/run/docker.sock` option in the docker run command enables the DooD functionality by giving the container access to the host's Docker socket.

## What's Your ETH CTF
This platform was used to host the WhatyourETH CTF, a project developed as part of the 12th K-Shield Junior Vulnerability Analysis Course. WhatyourETH CTF focuses on Ethereum and smart contract vulnerabilities, providing participants with hands-on experience in identifying and exploiting weaknesses in blockchain technologies.

## Acknowledgements
- Original CTFd project: [CTFd/CTFd](https://github.com/CTFd/CTFd)
- Docker plugin: [andyjsmith/CTFd-Docker-Plugin](https://github.com/andyjsmith/CTFd-Docker-Plugin)
