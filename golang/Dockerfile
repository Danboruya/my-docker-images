FROM golang:1.15.6

RUN apt update \
  && apt install -y vim

RUN adduser golang
WORKDIR /home/golang/go/src/work
RUN chown -R golang:golang /home/golang/go
USER golang

ENV HOME /home/golang
ENV GOPATH /home/golang/go
ENV GO111MODULE on
COPY .devcontainer/.bashrc /home/golang/