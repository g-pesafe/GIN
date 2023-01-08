FROM ubuntu:16.04


RUN add-apt-repository ppa:deadsnakes/ppa \
    apt-get update \
    apt-get install python3.6 \
    apt-get update -y && \
    apt-get install -y  python-pip python-dev curl 


   
COPY . /app
WORKDIR /app
RUN pip3 install -r requirements.txt






HEALTHCHECK --interval=10s --timeout=30s CMD curl --fail http://localhost:5000/ || exit 1





ENTRYPOINT ["python"]
CMD ["app.py"]

