FROM python:3.7-slim

RUN apt update \
  && apt install -y vim git

RUN adduser python
WORKDIR /home/python/work
RUN chown -R python:python /home/python/work
USER python

ENV HOME /home/python
COPY .devcontainer/.bashrc /home/python/