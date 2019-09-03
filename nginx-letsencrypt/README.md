# Details
This Docker Compose file bundles an *Nginx Reverse Proxy* and a *Letsencrypt* companion containers thus a production-grade HTTP server with virtual hosts can be spin up quickly.

Here is a quick schema:

![Nginx Letsencrypt Schema](schema.png "Nginx Letsencrypt Schema")
([credits](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion/blob/master/schema.png))

There are two example web application in this file. One is an `examplecom` named static web page served via *Nginx* (the usual not the reverse one) and one is an `examplewp` named *Wordpress* connected to a *MySQL* database. *Nginx Reverse Proxy*, forwards the packets to the `examplecom` and `examplewp` with respect to their virtual host parameters. Virtual hosts are set via `VIRTUAL_HOST` environment variable. This environment variables must be set for each web application that wanted to be proxied.

There are many environment variables that can be set for *Nginx Reverse Proxy*. Here is a quick list:

- ENABLE_IPV6
- VIRTUAL_PORT
- VIRTUAL_HOST
- VIRTUAL_PROTO
- VIRTUAL_ROOT
- DEFAULT_HOST

Check the [image repository](https://github.com/jwilder/nginx-proxy) for more information.

And a quick list of environment variables can be set for *Letsencrypt*:

- DEFAULT_EMAIL
- LETSENCRYPT_HOST
- LETSENCRYPT_EMAIL
- DHPARAM_BITS

Check the [image repository](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion) for more information.

