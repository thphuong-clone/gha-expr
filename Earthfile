VERSION 0.8

FROM alpine:3.19

build:
    RUN echo "Hello, world!" > /hello.txt

image:
    COPY +build/hello.txt /hello.txt

    ARG MY_ARG
    SAVE IMAGE my-alpine-${MY_ARG:-mmm}:3.19
