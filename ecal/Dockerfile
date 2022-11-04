FROM ubuntu:22.04

RUN apt-get update
RUN apt-get install software-properties-common -y
RUN add-apt-repository ppa:ecal/ecal-latest
RUN apt-get update
RUN apt-get install ecal -y

# Network config for cloud usage
RUN sed -i "s/network_enabled           = false/network_enabled           = true/g" /etc/ecal/ecal.ini

