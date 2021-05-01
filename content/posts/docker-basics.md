--- 
draft: true
date: 2021-05-01T17:41:14+02:00
title: "Docker Basics"
tags: ['docker']
categories: ['coding']
---
It has been quite a while!

Some quick recipes on using Docker.

Quite often, I need to test few thing in a controlled environment, nothing is easier than starting a virtual machine in interactive mode. For example, you can do:
```bash
docker run -v $(pwd):/root -it ubuntu:latest  /bin/bash
```
This command will:
 - run docker interactively (you will get a `pseudo-tty` with `stdin`)
 - start an Ubuntu image
 - mount the current directory in `/root`
 - the container will be automatically removed if existing
