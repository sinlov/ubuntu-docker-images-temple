# This dockerfile uses the sameersbn/ubuntu:14.04 image
# VERSION 1
# Author: sinlov
# Command format: Instruction [arguments / command]

FROM sameersbn/ubuntu:14.04.20180124

MAINTAINER  sinlov sinlovgmppt@gmail.com

RUN cp /etc/apt/sources.list /etc/apt/sources.list.bak
COPY ./sources.list /etc/apt/

# RUN apt-get update
# RUN apt-get install -y curl
RUN apt-get autoclean \
  && apt-get clean \
  && apt-get autoremove \
  && rm -rf /var/lib/apt/lists/*

EXPOSE  80

ENTRYPOINT ["tail", "-F", "/var/log/faillog"]
CMD ["-F", "/var/log/faillog"]

# ENV

# ADD

# COPY

# ENTRYPOINT

# VOLUME

# USER

# WORKDIR

# ONBUILD