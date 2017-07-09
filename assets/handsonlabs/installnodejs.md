## Hands On Labs

- Oracle Code Sydney July 2017

### 1. Install NodeJS

This section provides instructions for you to install Node.js. 
The Node.js install is required to run the MedRec application.

Note: I used the Ubuntu 16.04 Linux distribution, you may need to adjust the commands according to that required by your target operating system. For instance, if using other Fedora based OS then yum install of apt-get.

The first step is to checkl to see if you already have Node.js installed.
In case you know that you have already have it installed, then skip and move to the next stage.
If you are unsure, continue with the following:

Validate the current version of the Node.js software (if installed):

*nodejs --version*   or *node --version*

### 1.1 Install NodeJS (if not already installed)

*sudo apt-get install curl -y*
*sudo curl -sL https://deb.nodesource.com/setup_4.x | sudo -E bash –*
*sudo apt-get install nodejs -y *

Validate the NodeJS installation:

*nodejs --version* or *node --version*

You should get a valid version returned. 
Note: I used NodeJS version 4.8.0 while building this application.

For more information about using NodeJS [Visit Nodejs.org](https://nodejs.org/en/download/). 

* No warranty expressed or implied.  Software is as is.
* [MIT License](http://www.opensource.org/licenses/mit-license.html)

<hr />
<center>
<a href="../../handsonlabs" class="btn" >Back to Hands On Lab Menu</a>
<center />
<hr />

