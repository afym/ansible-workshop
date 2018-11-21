FROM ubuntu:18.04

MAINTAINER "techbrain"

ARG ANSIBLE_HOME=/home/ansible
ARG ANSIBLE_ETC=/etc/ansible
ENV ANSIBLE_CONFIG /etc/ansible/ansible.cfg

RUN apt update && \
     apt install software-properties-common -y && \
     apt-add-repository --yes --update ppa:ansible/ansible && \
     apt update && mkdir /home/ansible && \
     apt install ansible -y

WORKDIR /home/ansible