# docker-kubectl
Smallest possible kubectl Docker image

![Docker Automated build](https://img.shields.io/docker/automated/millergeek/kubectl.svg)

![Docker Build Status](https://img.shields.io/docker/build/millergeek/kubectl.svg)

![MicroBadger Size](https://img.shields.io/microbadger/image-size/millergeek/kubectl.svg)

![MicroBadger Layers](https://img.shields.io/microbadger/layers/millergeek/kubectl.svg)


## Instructions
If running in a pod authentication to the Kubernetes API should be automatic.
Otherwise, mount a config file to `/.kube/config` in the container.

## Example
```
docker run -p 8001:8001 -v $PWD/.kube/config:/.kube/config:ro millergeek/kubectl proxy
Starting to serve on 127.0.0.1:8001
```
