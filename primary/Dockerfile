FROM golang:1.14

RUN apt-get update && apt-get install -y ca-certificates make bash tar gzip curl gcc g++

RUN apt-get install -y git
RUN apt-get install -y git-lfs

RUN go get gotest.tools/gotestsum
