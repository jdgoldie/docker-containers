#
# MongoDB Install
#
FROM ubuntu:12.10
 
# Update the apt-sources
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 7F0CEB10 
RUN echo 'deb http://downloads-distro.mongodb.org/repo/ubuntu-upstart dist 10gen' | tee /etc/apt/sources.list.d/10gen.list 
RUN apt-get update -y
RUN apt-get install -y mongodb-10gen
RUN mkdir -p /data/db
 
# Expose the port
EXPOSE 27017
 
# Container starts mongod
ENTRYPOINT ["usr/bin/mongod"]