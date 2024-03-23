FROM debian

WORKDIR /app

RUN apt update
RUN apt upgrade 
RUN apt -y install vim
RUN apt -y install net-tools
RUN apt -y install iproute2
RUN apt -y install inetutils-ping
RUN apt -y install bzip2
RUN apt -y install wget
RUN apt -y install gcc
RUN apt -y install make
RUN apt -y install libgmp3-dev
RUN apt -y install postgresql 
RUN apt -y install curl


RUN wget https://download.strongswan.org/strongswan-5.9.1.tar.bz2
RUN tar xjf strongswan-5.9.1.tar.bz2
WORKDIR /app/strongswan-5.9.1

RUN <<EOT
./configure --prefix=/usr --sysconfdir=/etc
EOT

RUN make

RUN make install

COPY ipsec.* /etc/.

WORKDIR /etc
