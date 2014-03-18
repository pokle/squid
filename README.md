squid
=====

Run squid as a caching proxy in a docker container:

    docker run -d -p 3128:3128 poklet/squid

And then time a few http requests through the proxy with something like:

    time curl --proxy http://localhost:3128 http://SOME-BIG-FILE
