### MongoDB Docker Container###

[![Docker Repository on Quay.io](https://quay.io/repository/jdgoldie/mongo-db/status "Docker Repository on Quay.io")](https://quay.io/repository/jdgoldie/mongo-db)

Installs MongoDB on 64-bit Ubuntu.  A prebuilt image is available at quay.io.

    docker pull quay.io/jdgoldie/mongo-db

Usage:
    
    docker run -d -p 27017:27017 -v /path/to/mongo/data/db:/data/db quay.io/jdgoldie/mongo-db:latest

Omit the `-v` option if you don't want the data persisted outside the container.

##### Current Configuration #####

* Ubuntu 13.10
* MongoDB 2.4.9

Copyright &copy; 2014 Joshua Goldie <a href="https://twitter.com/jdgoldie" class="twitter-follow-button" data-show-count="false" data-dnt="true">Follow @jdgoldie</a>
<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+'://platform.twitter.com/widgets.js';fjs.parentNode.insertBefore(js,fjs);}}(document, 'script', 'twitter-wjs');</script>
