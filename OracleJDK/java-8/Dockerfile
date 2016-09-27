# LICENSE CDDL 1.0 + GPL 2.0
#
# Copyright (c) 2015 Oracle and/or its affiliates. All rights reserved.
#
FROM oraclelinux:latest

MAINTAINER Bruno Borges <bruno.borges@oracle.com>

ENV JAVA_PKG=server-jre-8u*-linux-x64.tar.gz 
ENV JAVA_HOME=/usr/java/default 
ENV PATH=$PATH:/usr/java/default/bin

ADD server-jre-8u*-linux-x64.tar.gz  /usr/java/

RUN mv $(ls -1 -d /usr/java/*) /usr/java/default
