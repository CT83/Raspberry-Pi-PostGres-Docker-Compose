# Spin up a PostGres Docker Container on the RPi in 2 minutes! 
## Raspberry-Pi-PostGres-Docker-Compose

Installing things is difficult! But, it does not need to be. 
[Tobias](https://tobias.hargesheimer.ws/) and me (mostly just Tobias) have already made this easy for you. 

This is a Docker Starter Pack thingy to help you _up_ a PostGreSQL Database on your Raspberry Pi within seconds. 

🐳 

Note, this assumes that you have a gentle grasp of what Docker Compose and Containerization are, so stay put for the rodeo!


## Setup
1. [Install Docker and Docker compose on the Raspberry Pi]( https://dev.to/rohansawant/installing-docker-and-docker-compose-on-the-raspberry-pi-in-5-simple-steps-3mgl)
2. Clone the [repo](https://github.com/CT83/Raspberry-Pi-PostGres-Docker-Compose) which contains the Compose file `git clone https://github.com/CT83/Raspberry-Pi-PostGres-Docker-Compose.git`
2. Checkout the postgresql.conf, and configure  `listen_addresses` accordingly. By default, the container will be open to all users on the port *5432*.
3. `sudo docker-compose up --build -d` _Up_ the container.

The container is at **<IP>:5432** with password _password@7979_. You can change this in the [docker-compose.yml](https://github.com/CT83/Raspberry-Pi-PostGres-Docker-Compose/blob/master/docker-compose.yml).
Now, you can treat this like a full fledged PostGres server and do your PG-Admin Stuff. 😇

Also, note that the PostGres Server can be accessed by any device on the network! 
Use this to build a _truly decentralized off-site infrastructure_ where each container runs on a separate low powered Raspberry Pi Zero, maybe?

### Credits
This would have been impossible without the base image created by [Tobias H.](https://github.com/Tob1asDocker). 

*I just added the docker-compose and a conf to allow other network hosts to connect to it*

You can check it out [here](
https://github.com/Tob1asDocker/rpi-postgresql)