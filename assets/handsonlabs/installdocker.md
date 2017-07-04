# Anki-Medrec APIs


## Installation

This section will help you deploy the docker software that can be optionally used to run the MedRec applciations.

### 1. Install Docker.

The first step is to ensure that you have installed NodeJS, MongoDB and Git in your environment. In case you know that you have already installed them, feel free to move to step number 2. Otherwise if you are unsure, continue with the following assessment:

Validate the installation of the required components (one at a time):
```
nodejs --version
mongo --version
git --version
```

#### 1.1 Install Docker (if not already installed)

```
sudo apt-get install curl -y
sudo curl -sL https://deb.nodesource.com/setup_4.x |
sudo -E bash –
sudo apt-get install nodejs -y 
```
Validate the NodeJS installation:
```
sudo docker --version
```
You should get a valid version. I used NodeJS version 4.8.0 while building this application.
---
add docker to sudoers
---

<br>

#### What next? 

If you want to move your application into the Cloud, consider Oracle Application Container Cloud Service as a simple way to fast-track its enablemnet and future scalability [Click here for more information](https://cloud.oracle.com/acc).

<br>
<br>

* No warranty expressed or implied.  Software is as is.
* [MIT License](http://www.opensource.org/licenses/mit-license.html)



<hr />
<a href="handsonlabs" class="btn" >Back to Hands On Lab Menu</a>
<hr />

