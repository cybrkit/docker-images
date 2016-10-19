# LICENSE CDDL 1.0 + GPL 2.0
#
# Copyright (c) 2015 Oracle and/or its affiliates. All rights reserved.
#
FROM oraclelinux:latest

MAINTAINER cybrkit <cybrkit@gmail.com>

ENV JAVA_PKG=server-jre-8u*-linux-x64.tar.gz 
ENV JAVA_HOME=/usr/java/default 
ENV PATH=$PATH:/usr/java/default/bin

RUN curl -L "https://www.dropbox.com/s/ggfpy9hs3ybrkw1/server-jre-8u101-linux-x64.tar.gz?dl=1" -o "/tmp/server-jre-8u101-linux-x64.tar.gz"

RUN mkdir -p /usr/java/default/
RUN tar -xf /tmp/server-jre-8u101-linux-x64.tar.gz -C /usr/java/
RUN mv $(ls -1 -d /usr/java/*) /usr/java/default
RUN rm /tmp/server-jre-8u101-linux-x64.tar.gz
