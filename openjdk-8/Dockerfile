FROM nimusis/ubuntu-ko:16.04
 			 
# set default java environment variable
ENV JAVA_HOME=/usr/lib/jvm/default-jvm \
    PATH=${PATH}:/usr/lib/jvm/default-jvm/bin/

RUN apt-get update -y \
 && apt-get install -qq -y python-software-properties software-properties-common

RUN add-apt-repository ppa:openjdk-r/ppa -y \
 && apt-get update \
 && apt-get install -y --no-install-recommends openjdk-8-jdk \
 && ln -s java-8-openjdk-amd64  /usr/lib/jvm/default-jvm \
 && apt-get clean all
