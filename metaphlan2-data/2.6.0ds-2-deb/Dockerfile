FROM biocontainers/biocontainers:debian-stretch-backports
MAINTAINER biocontainers <biodocker@gmail.com>
LABEL    software="metaphlan2-data" \ 
    container="metaphlan2-data" \ 
    about.summary="data package for Metagenomic Phylogenetic Analysis" \ 
    about.home="https://bitbucket.org/biobakery/metaphlan2" \ 
    software.version="2.6.0ds-2-deb" \ 
    version="1" \ 
    about.copyright="2012-2016 Duy Tin Truong, Nicola Segata and Curtis Huttenhower" \ 
    about.license="expat" \ 
    about.license_file="/usr/share/doc/metaphlan2-data/copyright" \ 
    about.tags=""

ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && apt-get install -y metaphlan2-data && apt-get clean && apt-get purge && rm -rf /var/lib/apt/lists/* /tmp/*
USER biodocker
