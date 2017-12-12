FROM nimusis/ubuntu-ko:16.04
 			 
RUN apt-get update -y \
 && apt-get install -qq -y curl wget git make cmake autoconf automake pkg-config \
 && apt-get install -qq -y build-essential gcc g++ clang gdb valgrind ctags \
 && apt-get install -qq -y python python-dev python-pip \
 && apt-get install -qq -y python3 python3-dev python3-pip \
 && apt-get install -qq -y vim \
 && apt-get autoremove -y \
 && apt-get autoclean \
 && rm -rf /tmp/* /var/lib/apt/lists/* /var/tmp/*
