Dockerfiles for building various containers.

### MongoDB ###

Installs MongoDB on Ubuntu 12.10.  A prebuilt image is available at quay.io.

    docker pull quay.io/jdgoldie/mongo-db

Usage:
    
    docker run -d -p 27017:27017 -v /path/to/mongo/data/db:/data/db quay.io/jdgoldie/mongo-db:latest

Omit the `-v` option if you don't want the data persisted outside the container.







Copyright &copy; 2014 Joshua Goldie