## Hands On Labs

- Oracle Code Sydney July 2017

### Install MongoDB

This section provides instructions to install the MongoDB software. This software is required for the MedRec applciation.

Note: I use Ubuntu Linux distribution, adjust accordingly if using a different Operating System.
For instance, if using a Fedora based distribution,then use *yum* instead of *apt-get*. 

The first step is to check to see if you already have installed MongoDB installed in your environment. 
If it is already installed, then move to the next stage of the lab.
Otherwise if you are unsure, continue with the following steps:

- Validate the installation of the MongoDB component:
```
*mongo --version*
```
You should get a valid version returned otherwise install it as per below. 

- Install MongoDB
*sudo apt-get install mongodb -y*
```
- Validate the MongoDB installation:
```
*mongo --version*
```
Note: I used MongDB shell version 2.6.10 while building this application

For more information about installation of MongoDB on your operating system, please refer
[mongodb.com](https://docs.mongodb.com/manual/installation/?jmp=footer&_ga=2.106487168.2097534541.1499499275-2109307220.1499499275). 

* No warranty expressed or implied.  Software is as is.
* [MIT License](http://www.opensource.org/licenses/mit-license.html)

<hr />
<center>
<a href="../../handsonlabs" class="btn" >Back to Hands On Lab Menu</a>
<center />
<hr />


