### How to use?

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