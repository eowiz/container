FROM alpine:latest

RUN apk --update --no-cache add openjdk17-jre-headless docker bash

SHELL [ "/bin/bash", "-c" ]

ENV JAVA_HOME=/usr/lib/jvm/java-17-openjdk

WORKDIR /home

ENTRYPOINT ["/bin/bash"]