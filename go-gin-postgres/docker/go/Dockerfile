ARG GO_VERSION=1.20.5
ARG ALPINE_VERSION=3.18

FROM golang:${GO_VERSION}-alpine${ALPINE_VERSION}

WORKDIR /app

RUN apk add bash

RUN go install github.com/cosmtrek/air@latest

COPY src/go.mod .
COPY src/go.sum .
RUN go mod download