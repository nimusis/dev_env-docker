FROM nimusis/ubuntu-ko:16.04
 			 
# set default java environment variable
ENV JAVA_HOME=/usr/lib/jvm/default-jvm \
    PATH=${PATH}:/usr/lib/jvm/default-jvm/bin/

RUN add-apt-repository ppa:openjdk-r/ppa -y && \

    # update data from repositories
    apt-get update && \

    # upgrade OS
    apt-get -y dist-upgrade && \

    # install application
    apt-get install -y --no-install-recommends openjdk-8-jdk && \

    # fix default setting
    ln -s java-8-openjdk-amd64  /usr/lib/jvm/default-jvm && \

    # remove apt cache from image
    apt-get clean all