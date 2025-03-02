# Supply Chain Security 

1. Minimizing the Base Image Footprint

The process for building a container image looks straightforward on the surface level; however, the devil is often in the details. 

It may not be obvious to someone new to the topic to refrain from building a container image that is unnecessarily too large in size, riddled with vulnerabilities, and not optimized for container layer caching.

2. Picking a Base Image Small in Size

$ docker pull alpine:3.17.0
...
$ docker image ls alpine
REPOSITORY   TAG       IMAGE ID       CREATED       SIZE
alpine       3.17.0    49176f190c7e   3 weeks ago   7.05MB


You can further reduce the container image size and the attack surface by using a distroless image offered by Google. The following command downloads the latest tag of the container image gcr.io/distroless/static-debian11 and renders its details. 

The size of the container image is only 2.34MB:

$ docker pull gcr.io/distroless/static-debian11
...
$ docker image ls gcr.io/distroless/static-debian11:latest
REPOSITORY                          TAG       IMAGE ID       CREATED      \
  SIZE
gcr.io/distroless/static-debian11   latest    901590160d4d   53 years ago \
  2.34MB