# This dockerfile uses the Ubuntu 14.04 image
# VERSION 1
# Author: sinlov
# Command format: Instruction [arguments / command]

FROM ubuntu:14.04

MAINTAINER  sinlov sinlovgmppt@gmail.com

RUN cp /etc/apt/sources.list /etc/apt/sources.list.bak
COPY ./sources.list /etc/apt/

RUN apt-get update
RUN apt-get install -y iputils-ping \
   curl \
   vim \
   net-tools
RUN apt-get autoclean
RUN apt-get clean
# RUN apt-get autoremove

EXPOSE  80

CMD /bin/bash

# ENV

# ADD

# COPY

# ENTRYPOINT

# VOLUME

# USER

# WORKDIR

# ONBUILD