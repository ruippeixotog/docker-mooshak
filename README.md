# ruippeixotog/mooshak Docker image

This repository contains the Dockerfile for `ruippeixotog/mooshak`, a Docker image with [Mooshak](https://mooshak.dcc.fc.up.pt) - a system for managing programming contests online, including but not limited to user and team management, problem serving, solution uploading and automatic judging.

The image is currently unable to send emails while registering teams, which means users must be created manually through the folder system.

## How to run

Create a container from this image with:

```
docker run -d -p 8080:80 -v local_path_to_mooshak_data:/home/mooshak/data ruippeixotog/mooshak
```

## Ports

* **80** - The Mooshak web interface, available at */~mooshak*.

## Volumes

* **/home/mooshak/data** - A directory containing all Mooshak data and configurations.
