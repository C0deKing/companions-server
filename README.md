# Companions server docker setup (with docker-compose)

To set up a local companions server without having to do any local installation, follow these steps. This setup should work regardless of platform (Windows, Linux or OSX)

## Prerequisites

- [Docker](https://docs.docker.com/engine/install/)
- [docker-compose](https://docs.docker.com/compose/install/)


## Steps

- Clone this repository `git clone https://github.com/C0deKing/companions-server`
- Change into the companions-server directory `cd companions-server`
- Start the docker-compose services `docker-compose up`
    - NOTE: If you do not want to see the logs, do it with the detached (-d) option `docker-compose up -d`
- In a browser of your choice, navigate to [Companions](http://127.0.0.1:9100/smgr.html)


## Shut Down

When you are done using the companions server, you can run the `docker-compose down` command to shut down the docker containers. Companions uses docker volumes, so any data stored on the server should persist so long as you do not manually delete the docker volume.