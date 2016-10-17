# LICENSE CDDL 1.0 + GPL 2.0
#
# Copyright (c) 2015 Oracle and/or its affiliates. All rights reserved.
#
FROM oraclelinux:latest

MAINTAINER cybrkit <cybrkit@gmail.com>

ENV JAVA_PKG=server-jre-8u*-linux-x64.tar.gz 
ENV JAVA_HOME=/usr/java/default 
ENV PATH=$PATH:/usr/java/default/bin

ADD dl_jre.sh  /tmp/
RUN chmod u+x /tmp/dl_jre.sh
RUN /tmp/dl_jre.sh

RUN mv /tmp/server-jre-8u101-linux-x64.tar.gz /usr/java/
RUN mv $(ls -1 -d /usr/java/*) /usr/java/default
