FROM ubuntu:20.04
RUN apt-get update
RUN apt-get -y install curl 
ENV URL https://google.com/this-will-fail?secret-token=
CMD ["sh", "-c", "curl --head $URL$TOKEN"]