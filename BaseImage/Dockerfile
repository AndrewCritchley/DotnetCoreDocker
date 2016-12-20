FROM ubuntu:16.10
MAINTAINER Andrew Critchley

RUN apt-get update
RUN apt-get install -y dirmngr && apt-get install -y apt-transport-https
RUN echo "deb [arch=amd64] https://apt-mo.trafficmanager.net/repos/dotnet-release/ yakkety main" > /etc/apt/sources.list.d/dotnetdev.list
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 417A0893
RUN apt-get update && apt-get install -y dotnet-dev-1.0.0-preview2.1-003177
RUN apt-get install -y ffmpeg

WORKDIR /app