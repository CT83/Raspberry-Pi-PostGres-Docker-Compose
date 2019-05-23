# Raspberry-Pi-PostGres-Docker-Compose
A simple way to run a PostGres database on the Raspberry Pi.

## Setup
1. [Install Docker and Docker compose on the Raspberry Pi](https://gist.github.com/CT83/0a3825402edf9ed1d6af951da5f768d1)
2. Checkout the postgresql.conf, and configure  `listen_addresses` accordingly.
3. `sudo docker-compose up --build -d` _Up_ the container.
