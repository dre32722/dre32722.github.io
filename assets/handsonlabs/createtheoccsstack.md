## Hands On Labs

- Oracle Code Sydney July 2017

### Create the OCCS Stack definition and deploy the container

As an alternative to running the APIs locally we may decide to deploy into the Oracle Public Cloud.
The Oracle Container Cloud Service (OCCS) provides a runtime environment for your Docker containers (essentiually Bring Yopur Own Container)

This assumes the user has access to the Oracle Container Cloud Service and involves the following;
- login to OCCS 
- create stack in OCCS using yml file
- deploy the stack
- access the apis - url 

Copy the contents of the occsstack.myl file. 
We will use this content to define our stack inside the OCCS environment.

<img src="./img/createtheoccsstack-0.PNG" />

Login to the Oracle Cloud using the credentials you have received / used during the  sign up process for the Oracle Cloud trial. 

Note: If you see no services then you will need to click the customise Dashboard to make the services of interest visible on the Dashboard.

From the Dashboard click the Container (not the Application Container) link.

<img src="./img/createtheoccsstack-1.PNG" />

Click the Open Service Console button

<img src="./img/createtheoccsstack-2.PNG" />

Click the Create Service button.
Give the service instance a name and specify the number of nodes you want in your Container runtime environment. NOTE : **You will need a minimum of two nodes as one node is dedicated to the Container Console.**
Also make sure you remember the username / password you specify as this is required for access to the container console.

<img src="./img/createtheoccsstack-3.PNG" />

Assuming you have created a service instance - click the hamburger menu on the far right and choose Container Console.

<img src="./img/createtheoccsstack-4.PNG" />

You will see an Insecure Connection Message.
Click the Advanced link and choose to continue.

<img src="./img/createtheoccsstack-5.PNG" />

Login to the Container Console using the credentials you used when you created the Service Instance.

<img src="./img/createtheoccsstack-6.PNG" />

Explore the Container Console

<img src="./img/createtheoccsstack-7.PNG" />

Click Stacks in the Left Pane and Click New Stack button (top right)

<img src="./img/createtheoccsstack-8.PNG" />

The console provides you with a couple of options.
- Drag and drop from the services on the right to create your stack, or,
- Click the Advanced Editor link

Click the Advanced Editor link

<img src="./img/createtheoccsstack-9.PNG" />

Paste the contents of the occsstack.yml file you copied earlier.

<img src="./img/createtheoccsstack-10.PNG" />

Your stack definition should look as follows.
Click Done.

<img src="./img/createtheoccsstack-11.PNG" />

Give your Stack a name under the Stack Name title (eg MedRecOCCS).

<img src="./img/createtheoccsstack-12.PNG" />

Your stack should appear in the list of available stacks.

<img src="./img/createtheoccsstack-13.PNG" />

Before you deploy the stack, click the Resource Pool from left menu.
Note that the default pool has the hosts that you specified when you created the service minus the one node allocated to the admin / console function. When you deploy a stack you need to specify the resource pool.

Click the Active Hosts section within the default Resource Pool.

<img src="./img/createtheoccsstack-14.PNG" />

You should now see the worker node hosts that are part of your 'default' Resource Pool.

<img src="./img/createtheoccsstack-15.PNG" />

Click on the IP address to see the public IP address of the various hosts.
Depending on which worker node is used for the docker stack deployment you will need to get the IP address to test the SwaggerUI.

<img src="./img/createtheoccsstack-16.PNG" />


<img src="./img/createtheoccsstack-17.PNG" />

<img src="./img/createtheoccsstack-18.PNG" />

<img src="./img/createtheoccsstack-19.PNG" />

<img src="./img/createtheoccsstack-20.PNG" />

<img src="./img/createtheoccsstack-21.PNG" />

<img src="./img/createtheoccsstack-22.PNG" />

<img src="./img/createtheoccsstack-23.PNG" />

<img src="./img/createtheoccsstack-24.PNG" />

<img src="./img/createtheoccsstack-25.PNG" />

<img src="./img/createtheoccsstack-26.PNG" />

<img src="./img/createtheoccsstack-27.PNG" />

* No warranty expressed or implied.  Software is as is.
* [MIT License](http://www.opensource.org/licenses/mit-license.html)

<hr />
<center>
<a href="../../handsonlabs" class="btn" >Back to Hands On Lab Menu</a>
<center />
<hr />

