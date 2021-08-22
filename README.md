# simple-dind

Simple Docker-in-Docker (dind) setup. Can be adapted to use with various CI runners as an alternative to mounting the docker socket from the host.

## Getting Started

```bash
docker-compose up
docker-compose exec dev docker info
```

## Credits

Based on the [official dind documentation](https://hub.docker.com/_/docker).

