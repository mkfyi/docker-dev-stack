# docker-dev-stack

Technology stack for the development of backend applications / microservices.

## Usage

1. Clone the repository: `git clone https://github.com/mkfyi/docker-dev-stack`
2. Naviagte into the repository: `cd docker-dev-stack`
3. Bootstrap the stack: `./bootstrap up`

## Tech Stack

[docker_adminer]: https://hub.docker.com/_/adminer
[docker_rmq]: https://hub.docker.com/_/rabbitmq
[docker_traefik]: https://hub.docker.com/_/traefik
[docker_mariadb]: https://hub.docker.com/_/mariadb

|Service|Version|
|---|---|
|[MariaDB][docker_mariadb]|`latest`|
|[Adminer][docker_adminer]|`latest`|
|[RabbitMQ][docker_rmq]|`3.12`|
|[Traefik][docker_traefik]|`2.10`|

### Traefik

If used, the dashboard can be accessed under <http://traefik.docker.localhost>. In addition, the following URLs are provided:

- <http://amqp.docker.localhost>
- <http://sql.docker.localhost>

### Credentials

|Service|Username|Password|
|---|---|---|
|MariaDB|`root`|`secret`|
|RabbitMQ|`admin`|`secret`|

## Credits

- [Lukáš Hron (@lukashron)](https://github.com/lukashron) - for his [dark theme](https://github.com/lukashron/adminer-dark-theme) for Adminer

## LICENSE

[docker-dev-stack](https://github.com/mkfyi/docker-dev-stack) is [MIT licensed](LICENSE.md).
