#Pull JDK image
FROM myantdeploy:v1

MAINTAINER Arun Nair <arun.b.nair@accenture.com>


RUN mkdir -p $HOME/opt/apache-ant/lib
#ENV ANT_HOME $HOME/opt/apache-ant
WORKDIR $HOME/opt/apache-ant/

ENV ANT_HOME  /usr/share/ant/
ENV PATH $PATH:$ANT_HOME/bin

# Add build files to ANT directories

ADD ant-salesforce.jar $HOME/opt/apache-ant/lib/
ADD build.xml $HOME/opt/apache-ant/
ADD build.properties $HOME/opt/apache-ant/
ADD package.xml $HOME/opt/apache-ant/

# Test out a sample retrieval of metadata

RUN ant retrieve

# Define default command.
CMD ["bash"]