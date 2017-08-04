## Hands On Labs

- Oracle Code Sydney July 2017

### Installation of Docker-Compose 

This section provides instructions to install docker-compose. Compose is a tool for defining and running multi-container Docker applications. In our case we will have a Docker container for the MedRec Node.js web application and another container for the MongoDB database. 

Docker for Mac, Docker for Windows, and Docker Toolbox include Docker Compose, so **most Mac and Windows users do not need to install Docker Compose separately**.

If you do need to install docker-compose on your platform, please follow the information provided at the following site for your platform specific installation instructions [Docker-Compose install Info](https://docs.docker.com/compose/install/).

### Installation of Docker-Compose on Ubuntu 16.04

Docker-Compose Instructions taken from: 
[Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-install-docker-compose-on-ubuntu-16-04) 

```
sudo curl -o /usr/local/bin/docker-compose -L "https://github.com/docker/compose/releases/download/1.11.2/docker-compose-$(uname -s)-$(uname -m)" 
```

```
sudo chmod +x /usr/local/bin/docker-compose
```

Verify the installation was successful by running:

```
docker-compose -v
```

You should see something returned like the following: **docker-compose version 1.11.2, build dfed245**


* No warranty expressed or implied.  Software is as is.
* [MIT License](http://www.opensource.org/licenses/mit-license.html)

<hr />
<center>
<a href="../../handsonlabs" class="btn" >Back to Hands On Lab Menu</a>
<center />
<hr />

