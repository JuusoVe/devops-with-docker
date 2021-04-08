FROM ubuntu:18.04

WORKDIR /usr/src/app

COPY curl.sh .

RUN apt-get update; apt-get -y install curl

CMD sh -c ./curl.sh

