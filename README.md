# Raspberry-Pi-PostGres-Docker-Compose

Installing things is difficult! But, it does not need to be.

This is a Docker and Docker-Compose Starter Pack thingy to help you _up_ a PostGreSQL Database on your Raspberry Pi within seconds. 


## Setup
1. [Install Docker and Docker compose on the Raspberry Pi]( https://dev.to/rohansawant/installing-docker-and-docker-compose-on-the-raspberry-pi-in-5-simple-steps-3mgl)
2. Checkout the postgresql.conf, and configure  `listen_addresses` accordingly. By default, the container will be open to all users on the port *5432*.
3. `sudo docker-compose up --build -d` _Up_ the container.
