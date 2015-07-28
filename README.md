# Docker PyCSW

PyCSW Docker image.

## Building image clonning this repository
Build image and run container (cloning this Git repository):

```bash
$ docker build -t geographica/pycsw:2.0-dev .
$ docker run --name pycsw -p 8086:8000 -it --rm geographica/pycsw:2.0-dev python /var/www/pycsw/csw.wsgi
```
Testing with a GetCapabilities request:

```bash
$ curl -v "http://localhost:8086/?service=CSW&version=2.0.2&request=GetCapabilities"
```

## Versions

Each version is a branch in GitHub and a tag in Docker Hub (TODO). These are the available versions:

- geographica/pycsw:2.0-dev


## DockerHub

TODO
