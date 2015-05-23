# Installing JDK 
FROM ubuntu:14.04
MAINTAINER Arun Nair <arun.b.nair@gmail.com>

# Install Java.
RUN \
  apt-get update && \
  apt-get install -y default-jdk && \
  rm -rf /var/lib/apt/lists/*
# If you re-use this dockerfile for a specific implementation
# Comment out the following lines
# WORKDIR /data
# ENV JAVA_HOME /usr/lib/jvm/java-7-openjdk-amd64

CMD ["bash"]
