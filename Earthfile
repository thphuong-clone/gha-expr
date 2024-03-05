VERSION 0.8

FROM alpine:3.19

build:
    RUN echo "Hello, world!" > /hello.txt

    SAVE ARTIFACT /hello.txt

image:
    COPY +build/hello.txt /

    ARG MY_ARG
    ARG TAG

    SAVE IMAGE my-alpine${MY_ARG}:${TAG:-latest}
