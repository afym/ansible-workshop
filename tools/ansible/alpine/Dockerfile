FROM python:3.7.1-alpine3.8

# VERSIONS : https://pypi.org/project/ansible/#history
RUN apk add --update git bash openssh gcc musl-dev openssl-dev sshpass
RUN apk add --no-cache --virtual .pynacl_deps build-base python3-dev libffi-dev
RUN pip install --upgrade pip
RUN pip install --upgrade setuptools
RUN pip install ansible==2.7.2
