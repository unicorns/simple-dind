# simple-dind

Simple Docker-in-Docker (dind) setup. Can be adapted to use with various CI runners as an alternative to mounting the docker socket from the host.

## Getting Started

```bash
docker-compose up
docker-compose exec dev docker info
```

## Caveats

Currently all volume mounts are from witin the `docker` container that runs the docker daemon. In order to mount from the `dev` container, a shared directory between `dev` and `docker` must be set up (can be done using shared volume mounts or shared bind mounts to the host).

## Credits

Based on the [official dind documentation](https://hub.docker.com/_/docker).

