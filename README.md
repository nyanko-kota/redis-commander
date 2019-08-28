# redis-commander
[![Docker Automated build](https://img.shields.io/docker/automated/nyankokota/redis-commander.svg?style=flat)](https://hub.docker.com/r/nyankokota/redis-commander/)
[![Docker Pulls](https://img.shields.io/docker/pulls/nyankokota/redis-commander.svg?style=flat)](https://hub.docker.com/r/nyankokota/redis-commander/)
[![MIT License](https://img.shields.io/github/license/nyanko-kota/redis-commander.svg?style=flat)](https://github.com/nyanko-kota/redis-commander/blob/master/LICENSE.txt)

### How to use

```
version: '3'
services:
    redis-commander:
      container_name: "redis-commander"
      image: nyankokota/redis-commander:latest
      links:
          - redis:redis
      ports:
          - "8080:8080"
      command: --redis-host redis --port 8080
```
