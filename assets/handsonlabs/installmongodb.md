## Hands On Labs

- Oracle Code Sydney July 2017

### Install MongoDB

This section provides instructions to install the MongoDB software. This software is required for the MedRec application.

For more information about installation of MongoDB on your operating system, please refer
[Install MongoDB Community Edition](https://docs.mongodb.com/manual/administration/install-community/)
or for other editions, please refer;
[Install Other Editions of Mongodb](https://docs.mongodb.com/manual/installation/?jmp=footer&_ga=2.106487168.2097534541.1499499275-2109307220.1499499275). 

### Install MongoDB on Ubuntu 16.04

The first step is to check to see if you already have installed MongoDB installed in your environment. 
If it is already installed, then move to the next stage of the lab. 
Otherwise if you are unsure, continue with the following steps.

Once MongoDB is installed the file /etc/init.d/mongodb holds useful information for the start / stop of the mongoDB service. To determine the database file location refer /etc/mongodb.conf 

- Validate the installation of the MongoDB component:
```
/usr/bin/mongod --version
```
You should get a valid version returned otherwise install it as per below.
I used v2.6.10 .

- Validate the installation of the MongoDB Client component:
```
mongo --version
```
You should get a valid version returned otherwise install it as per below. 

- Install MongoDB
```
sudo apt-get install mongodb -y
```
- Validate the MongoDB installation:
```
/usr/bin/mongod --version
```
- Validate the MongoDB Client installation:
```
mongo --version
```
Note: I used MongDB shell version 2.6.10 while building this application

* No warranty expressed or implied.  Software is as is.
* [MIT License](http://www.opensource.org/licenses/mit-license.html)

<hr />
<center>
<a href="../../handsonlabs" class="btn" >Back to Hands On Lab Menu</a>
<center />
<hr />


