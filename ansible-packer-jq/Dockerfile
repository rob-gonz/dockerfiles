
# By default uses new Minimal Ubuntu 18.04 LTS image for docker
FROM ubuntu:18.04

MAINTAINER Robert Gonzalez <rob.d.gonz[@t]gmail.com>

ARG PACKER_VER=1.4.2

RUN apt-get update \
    && apt-get install -y jq git openssl ansible unzip \
    && wget -O /tmp/packer.zip "https://releases.hashicorp.com/packer/${PACKER_VER}/packer_${PACKER_VER}_linux_amd64.zip" \
    && unzip -o /tmp/packer.zip -d /usr/local/bin \
    && rm -f /tmp/packer.zip \
    && rm -rf /var/lib/apt/lists/*



