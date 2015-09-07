# fakes3-docker
Minimal (22.78 Mb) fakes3 Docker image based on Alpine Linux.

Exposes port 80 and uses `/srv/fakes3` as a volume for persistance. Uses `/usr/bin/fakes3` as entrypoint with the default flags `-r /srv/fakes3 -p 80`. You can override those flags by providing them when starting the container:

```
docker run -d -v /tmp/fakes3:/fakes3 -p :9999 fakes3 -r /fakes3 -p 9999
```

