FROM golang:1.14-alpine

RUN apk add --no-cache --update ca-certificates make bash tar gzip curl gcc g++

RUN apk add --no-cache git
RUN apk add --no-cache git-lfs

# GLIBC for Alpine linux, see https://github.com/sgerrand/alpine-pkg-glibc, Herumi BLS is linked against it.
RUN wget -q -O /etc/apk/keys/sgerrand.rsa.pub https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub
RUN wget https://github.com/sgerrand/alpine-pkg-glibc/releases/download/2.31-r0/glibc-2.31-r0.apk
RUN apk add glibc-2.31-r0.apk

RUN go get gotest.tools/gotestsum
