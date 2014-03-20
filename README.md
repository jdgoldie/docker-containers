### MongoDB Docker Container###

[![Docker Repository on Quay.io](https://quay.io/repository/jdgoldie/mongo-db/status "Docker Repository on Quay.io")](https://quay.io/repository/jdgoldie/mongo-db)

Installs MongoDB on 64-bit Ubuntu.  A prebuilt image is available at quay.io.

    docker pull quay.io/jdgoldie/mongo-db

Usage:
    
    docker run -d -p 27017:27017 -v /path/to/mongo/data/db:/data/db quay.io/jdgoldie/mongo-db:latest

Omit the `-v` option if you don't want the data persisted outside the container.

##### Current Configuration #####

* Ubuntu 12.10
* MongoDB 2.4.9

Copyright &copy; 2014 Joshua Goldie