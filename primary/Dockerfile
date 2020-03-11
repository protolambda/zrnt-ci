FROM golang:1.14

RUN apk add --no-cache --update ca-certificates make bash tar gzip curl gcc g++

RUN apk add --no-cache git
RUN apk add --no-cache git-lfs

RUN go get gotest.tools/gotestsum
