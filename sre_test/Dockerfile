FROM ubuntu:latest
MAINTAINER Rajdeep Dua "dua_rajdeep@yahoo.com"
RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential
RUN mkdir /app
COPY . /app/
WORKDIR /app
RUN pip install .
RUN pip install -r requirements.txt
RUN myapi init
ENTRYPOINT ["/usr/local/bin/flask","run"]