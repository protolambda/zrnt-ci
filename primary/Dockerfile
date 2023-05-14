FROM golang:1.20

RUN apt-get update && apt-get install -y ca-certificates make bash tar gzip curl gcc g++

RUN apt-get install -y git
RUN apt-get install -y git-lfs

RUN go install gotest.tools/gotestsum@latest
RUN go install github.com/golangci/golangci-lint/cmd/golangci-lint@latest
