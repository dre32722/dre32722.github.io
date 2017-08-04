## Hands On Labs

- Oracle Code Sydney July 2017

### 1. Install NodeJS

The Node.js install is required to run the MedRec application.
This section provides instructions for you to install Node.js. 
For your platform specific download and instructions please refer [Nodejs.org](https://nodejs.org/en/download/). 

Note: I used the Ubuntu 16.04 Linux distribution, and installed Node 4.8 when the application was built and tested. There are later versions of Node.js (eg 6.x) available. The following Node.js versions are currently supported on Oracle Application Container Cloud Servcie (ACCS) - 0.10, 0.12, 4.x, 6.x .

The MedRec application has been developed and tested using **Node 4.X**.
Please install Node 4.X to ensure compatibility when doing the Hands On Labs.

### 1.1 Install NodeJS on Ubuntu 16.04

Check to see if you already have Node.js installed.
In case you know that you have already have it installed, then skip and move to the next stage.

Because of a conflict with another package on Ubuntu, the executable from the Ubuntu repositories is called nodejs instead of node. Keep this in mind as you are running the software. 

``` nodejs --version ```

If you are unsure, continue with the following steps.
Validate the current version of the Node.js software (if installed):

``` 
sudo apt-get install curl -y
sudo curl -sL https://deb.nodesource.com/setup_4.x | sudo -E bash -
sudo apt-get install nodejs -y 
```

Validate the NodeJS installation:

``` nodejs --version ```

You should get a valid version returned. 

For more information about using NodeJS [Visit Nodejs.org](https://nodejs.org/en/download/). 

* No warranty expressed or implied.  Software is as is.
* [MIT License](http://www.opensource.org/licenses/mit-license.html)

<hr />
<center>
<a href="../../handsonlabs" class="btn" >Back to Hands On Lab Menu</a>
<center />
<hr />

