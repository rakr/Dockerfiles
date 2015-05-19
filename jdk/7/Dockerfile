# Installing JDK 
# Pull base image.
FROM ubuntu:14.04
MAINTAINER Arun Nair <arun.b.nair@accenture.com>

# Install Java.
RUN \
  apt-get update && \
  apt-get install -y default-jdk && \
  rm -rf /var/lib/apt/lists/*

# Define working directory.
# WORKDIR /data

# Define commonly used JAVA_HOME variable
# ENV JAVA_HOME /usr/lib/jvm/java-7-openjdk-amd64

# Define default command.
CMD ["bash"]