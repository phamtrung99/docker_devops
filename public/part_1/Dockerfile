FROM ubuntu:20.04
WORKDIR /usr/src/app
COPY web-script.sh .
RUN apt-get update
RUN apt-get install -y curl
RUN chmod +x web-script.sh
CMD ./web-script.sh
