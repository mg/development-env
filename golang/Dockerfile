FROM golang:1.21-rc-alpine

RUN adduser --disabled-password --gecos '' go
USER go
ENV GOOS="darwin" GOARCH="amd64" GOPATH="/home/go"
ENV PATH="$PATH:$GOPATH/bin"
WORKDIR "/home/go/src"
