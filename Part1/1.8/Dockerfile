FROM ubuntu:18.04
WORKDIR /myapp
COPY curler.sh  .
CMD ./curler.sh
RUN apt-get update
RUN apt-get install curl -y