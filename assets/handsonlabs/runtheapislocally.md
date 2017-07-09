## Hands On Labs

- Oracle Code Sydney July 2017

### Run the Node APIs locally

This section provides instructions to run the node application locally on your laptop.
First ensure that MongoDB is running

<img src="./img/runlocal1.PNG" />

Navigate to the ankimedrec-apis directory and run the following command.
This command will pull down the required library packages to support the application based on the contents of the package.json file.

*npm install*

You can ignore the npm WARN ankimedrec-swaggerui@1.0.0 No repository field message.

<img src="./img/runlocal1a.PNG" />

Next execute the command to start the node application.

*nodejs app.js* or *node app.js*

<img src="./img/runlocal2.PNG" />

You should see that the application is running and accepting request on localhost:3000

<img src="./img/runlocal3.PNG" />

Launch a web browser and point it to **localhost:3000**
You should see the SwaggerUI displayed as per the following screenshot.

<img src="./img/runlocal4.PNG" />


* No warranty expressed or implied.  Software is as is.
* [MIT License](http://www.opensource.org/licenses/mit-license.html)

<hr />
<center>
<a href="../../handsonlabs" class="btn" >Back to Hands On Lab Menu</a>
<center />
<hr />

