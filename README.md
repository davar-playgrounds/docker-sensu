[![HitCount](http://hits.dwyl.io/sangahco/sangahco/docker-sensu.svg)](http://hits.dwyl.io/sangahco/sangahco/docker-sensu)
[![Jenkins](https://img.shields.io/jenkins/s/https/dev.builder.sangah.com/job/sensu-prod.svg?style=flat-square)]()

# Server and Client for monitoring Docker containers

Docker images ready to run for Sensu server and client service.
The client has already a couple of plugins installed for monitoring docker containers, disk space and other few things.

## Requirements

First make sure *Docker* and *Docker Compose* are installed on the machine with:

    $ docker -v
    $ docker-compose -v

If they are missing, follow the instructions on the official website (they are not hard really...):

- [Docker CE Install How-to](https://docs.docker.com/engine/installation/)
- [Docker Compose Install How-to](https://docs.docker.com/compose/install/)


## How to Use

**Use the script `docker-auto.sh` to manage these services!**

    $ ./docker-auto.sh --help


## Settings Up the Environment

The following settings are available:

| Variable       | Description                                                             | Default |
|----------------|-------------------------------------------------------------------------|---------|
| SENSU_HOST     | The Sensu server host                                                   |         |
| SENSU_USER     | The username to access RabbitMQ                                         |         |
| SENSU_PASSWORD | The password to access RabbitMQ                                         |         |
| CLIENT_NAME    | The client name that will show up in uchiwa UI                          |         |
| CLIENT_IP      | The client IP that will be used by Sensu server to talk with the client |         |

(\*) *table generated with [tablesgenerator](http://www.tablesgenerator.com/markdown_tables)*
