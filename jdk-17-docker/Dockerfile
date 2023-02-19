FROM debian:stable-slim

RUN apt-get update && apt-get install -y \
       openjdk-17-jdk-headless \
       docker \
    && apt-get autoremove -y \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

RUN echo export JAVA_HOME=$(readlink -f /usr/bin/javac | sed 's:/bin/javac::') >> ~/.bashrc

WORKDIR /home

ENTRYPOINT ["/bin/bash"]