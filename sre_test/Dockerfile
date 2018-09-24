FROM ubuntu:latest
MAINTAINER Rajdeep Dua "dua_rajdeep@yahoo.com"
RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential
RUN mkdir /app
COPY . /app/
WORKDIR /app
RUN ls -al
RUN pip install -e .
RUN pip install -r requirements.txt
RUN myapi init
ENTRYPOINT ["python"]
CMD ["app.py"]
