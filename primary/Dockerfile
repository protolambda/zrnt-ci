FROM golang:1.12-alpine

RUN apk add --no-cache ca-certificates make tar gzip curl

RUN apk add --no-cache git
RUN apk add --no-cache git-lfs

RUN go get gotest.tools/gotestsum
