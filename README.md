# ![](https://github.com/CTFd/CTFd/blob/master/CTFd/themes/core/static/img/logo.png?raw=true)

## ![CTFd 3.5.0](https://github.com/CTFd/CTFd/tree/3.5.0)

CTFd is a Capture The Flag framework focusing on ease of use and customizability. It comes with everything you need to run a CTF and it's easy to customize with plugins and themes.

![CTFd is a CTF in a can.](https://github.com/CTFd/CTFd/blob/master/CTFd/themes/core/static/img/scoreboard.png?raw=true)

## ![andyjsmith/CTFd-Docker-Plugin](https://github.com/andyjsmith/CTFd-Docker-Plugin)

We used this plugin to provide individual ctf environment.

## Install

You can build image and use images with the following command:

`docker build -t ctfd .`

`docker run -d -p 80:8000 -v /var/run/docker.sock:/var/run/docker.sock --group-add [docker_group_id] ctfd`

or you can use Docker Compose with the following command from the source repository:

`docker compose build --no-cache`

`docker compose up`

Check out the [CTFd docs](https://docs.ctfd.io/) for [deployment options](https://docs.ctfd.io/docs/deployment/installation) and the [Getting Started](https://docs.ctfd.io/tutorials/getting-started/) guide
