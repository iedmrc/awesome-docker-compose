# Awesome Docker Compose
<p>
  <a href="https://twitter.com/iedmrc">
    <img alt="Twitter: iedmrc" src="https://img.shields.io/twitter/follow/iedmrc.svg?style=social" target="_blank" />
  </a>
  <img alt="Awesome badge" src="https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg" target="_blank" />
  <img alt="Made with love badge" src="https://img.shields.io/badge/Made%20With-Love-orange.svg" target="_blank" />
</p>

This *Awesome Docker Compose* repository consists of useful `docker-compose` files. A well-prepared Docker stack can be run  with just a single `docker-compose up -d` command thanks to the `docker-compose` files in this repository. 

For now, there are some `docker-compose` files created by me but looking for contributors. See [Contribution Guideline](CONTRIBUTING.md) for more information.

## Table of Contents

+ [Galois](galois)
+ [Nginx Reverse Proxy with Letsencrypt](nginx-letsencrypt)
+ [OpenVPN](openvpn)
+ [VROOM](vroom)

## Run

Make sure you have [Docker](https://docs.docker.com/install/) and [Docker Compose](https://docs.docker.com/compose/install/) installed on your local. Also don't forget to check *compose file* version matches with your Docker Compose and Docker versions.

After all, run the following command:

```sh 
docker-compose up -d
```

Here `-d` runs the stack in the background. If you don't want to run all the containers but some, do the following:

```sh 
docker-compose up -d service1 service2
```

### Destroy

To stop and remove the stack just give the following:

```sh 
docker-compose down
```

## Author

👤 **Ibrahim Ethem DEMIRCI**

Twitter: [@iedmrc](https://twitter.com/iedmrc) | Github: [@iedmrc](https://github.com/iedmrc) | Patreon: [@iedmrc](https://patreon.com/iedmrc)


Ibrahim's open-source projects are supported by his Patreon. If you found this project helpful, any monetary contributions to the Patreon are appreciated and will be put to good creative use.

## License

It is licensed under MIT License as found in the LICENSE file.