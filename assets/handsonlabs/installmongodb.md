# Anki-Medrec - External APIs - Node.js & MongoDB

This is an application provides a Swagger API documentation for the Anki-Medrec Platform project.  For more information, [visit this link](http://anki.medrec.oracleau.cloud).


## Installation

This sections will help you deploy the different packages required to run this Application. This includes: NodeJS, MongoDB and Git.

Note: I use Ubuntu Linux distribution, adjust accordingly if using other OS (e.g. "yum" if using Fedora based distributions).

### 1. Install MongoDB

The first step is to ensure that you have installed NodeJS, MongoDB and Git in your environment. In case you know that you have already installed them, feel free to move to step number 2. Otherwise if you are unsure, continue with the following assessment:

Validate the installation of the required components (one at a time):
```
mongo --version
```

#### 1.2 Install MongoDB (if not already installed):

```
sudo apt-get install mongodb -y
```

Validate the MongoDB installation:
```
mongo --version
```
You should get a valid version. I used MongDB shell version 2.6.10 while building this application

For more information about using MongoDB [visit to this page](https://redthunder.blog/2017/02/28/teaching-how-to-use-mongodb-and-expose-it-via-nodejs-apis/). 



#### What next? 

If you want to move your application into the Cloud, consider Oracle Application Container Cloud Service as a simple way to fast-track its enablemnet and future scalability [Click here for more information](https://cloud.oracle.com/acc).

<br>
<br>

* No warranty expressed or implied.  Software is as is.
* [MIT License](http://www.opensource.org/licenses/mit-license.html)


<hr />
<a href="handsonlabs" class="btn" >Back to Hands On Lab Menu</a>
<hr />


