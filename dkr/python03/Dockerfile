FROM ubuntu:16.04


RUN apt-get install --reinstall ca-certificates \
    apt-get install software-properties-common \
    add-apt-repository 'ppa:deadsnakes/ppa'  \
    apt-get update -y && \
    apt-get install -y python3.6  python-pip python-dev curl  
   


CMD python3 --version

