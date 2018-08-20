
# Java in Docker

This repo contains example of running a simple SpringBoot app in a Docker container.

Examples are based on the Docker images produced by the amazing [AdoptOpenJDK](https://adoptopenjdk.net/) project.

## Build

The [docker-compose.yml](docker-compose.yml) file contains configuration to build all containers.

To create the images:

```
> docker-compose build
```

## Run

To run the built images:


```
> docker-compose up
```

