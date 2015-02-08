FROM debian:wheezy

RUN apt-get update
RUN apt-get install -y wget
ADD salt.list /etc/apt/sources.list.d/salt.list
RUN wget -q -O- "http://debian.saltstack.com/debian-salt-team-joehealy.gpg.key" | apt-key add -
RUN apt-get update
RUN apt-get install -y salt-minion
