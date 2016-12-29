FROM ubuntu:latest

RUN apt-get update \
&& apt-get install -y golang-go

RUN rm /bin/sh && ln -s /bin/bash /bin/sh
RUN mkdir -p /opt/services/serviceA

WORKDIR /opt/services/serviceA
ADD test.go /opt/services/serviceA

EXPOSE 8080

CMD go run test.go

