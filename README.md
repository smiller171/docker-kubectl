# docker-kubectl
Smallest possible kubectl Docker image

![Docker Automated build](https://img.shields.io/docker/automated/scottmiller171/kubectl.svg)

![Docker Build Status](https://img.shields.io/docker/build/scottmiller171/kubectl.svg)

![MicroBadger Size](https://img.shields.io/microbadger/image-size/scottmiller171/kubectl.svg)

![MicroBadger Layers](https://img.shields.io/microbadger/layers/scottmiller171/kubectl.svg)


## Instructions
If running in a pod authentication to the Kubernetes API should be automatic.
Otherwise, mount a config file to `/.kube/config` in the container.

## Example
```
docker run -p 8001:8001 -v $PWD/.kube/config:/.kube/config:ro scottmiller171/kubectl proxy
Starting to serve on 127.0.0.1:8001
```
