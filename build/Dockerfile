from perl:latest

ADD . /opt/build
WORKDIR /opt/build

RUN apt-get update && \
	apt-get install libnet-ssleay-perl libio-socket-ssl-perl -y && \
	/opt/build/bake-modules

EXPOSE 5000
