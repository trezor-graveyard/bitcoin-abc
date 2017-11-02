FROM ubuntu:xenial
MAINTAINER slush@satoshilabs.com

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update && \
    apt-get -qy install curl g++-aarch64-linux-gnu g++-5-aarch64-linux-gnu gcc-5-aarch64-linux-gnu binutils-aarch64-linux-gnu \
          g++-5-multilib \
          gcc-5-multilib binutils-gold git-core pkg-config autoconf libtool automake faketime bsdmainutils ca-certificates python locales

ADD run_inside.sh /run.sh
RUN chmod +x /run.sh
