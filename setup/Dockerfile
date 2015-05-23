
#Pull JDK image
FROM ubuntu:14.04
# FROM arunintrade/install_jdk:v1
MAINTAINER Arun Nair <arun.b.nair@accenture.com>

# Install Java.
RUN apt-get update
RUN apt-get install -y default-jdk
  
# Define commonly used JAVA_HOME variable
ENV JAVA_HOME /usr/lib/jvm/java-7-openjdk-amd64

WORKDIR /home
ENV HOME /home
RUN mkdir -p $HOME/opt/apache-ant/lib


RUN apt-get -u install -y ant
# RUN wget http://archive.apache.org/dist/ant/binaries/apache-ant-1.8.4-bin.tar.gz

# RUN tar -xvzf apache-ant-1.8.4-bin.tar.gz && \
 # mv apache-ant-1.8.4 $HOME/opt/apache-ant

WORKDIR $HOME/opt/apache-ant/
#ENV ANT_HOME $HOME/opt/apache-ant
ENV ANT_HOME  /usr/share/ant/
ENV PATH $PATH:$ANT_HOME/bin


# Define default command.
CMD ["bash"]