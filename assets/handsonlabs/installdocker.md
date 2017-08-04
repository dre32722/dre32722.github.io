## Hands On Labs

Oracle Code Sydney July 2017

### Install Docker.

This section will help you deploy the docker software that can be optionally used to run the MedRec applications.

To find your platform specific install instructions go to [docker.com](https://www.docker.com).

### 1.1 Install Docker on Ubuntu 16.04

Steps taken from: [Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-16-04)


```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
sudo apt-get update
apt-cache policy docker-ce
sudo apt-get install -y docker-ce
```

Validate the docker installation and that the docker daemon is up and running:

```
sudo docker --version
```
```
sudo systemctl status docker
```
You should see: “Active: active (running) since…”

* No warranty expressed or implied.  Software is as is.
* [MIT License](http://www.opensource.org/licenses/mit-license.html)

<hr />
<center>
<a href="../../handsonlabs" class="btn" >Back to Hands On Lab Menu</a>
<center />
<hr />

