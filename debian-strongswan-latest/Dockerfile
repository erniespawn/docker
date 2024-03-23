FROM debian

WORKDIR /app

RUN apt update
RUN apt upgrade 
RUN apt -y install vim
RUN apt -y install net-tools
RUN apt -y install iproute2
RUN apt -y install inetutils-ping
RUN apt -y install strongswan 



COPY ipsec.* /etc/.

WORKDIR /etc
